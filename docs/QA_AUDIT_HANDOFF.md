# Walkthrough de Refatoração QA

Após o crivo implacável dos nossos três subagentes auditores, apliquei uma bateria de correções profundas no `index.html` visando a maturidade do sistema. O objetivo principal foi estancar vazamentos de acessibilidade, corrigir a fidelidade ao Design System e otimizar os ciclos da GPU na execução do JavaScript.

## Modificações Aplicadas

### 1. Governança do Design System (UI/UX)
- **Glassmorphism Corrigido:** Calibrei a Navbar e o Hero Card para respeitarem estritamente os tokens de opacidade e blur estabelecidos no `DESIGN.md`. A Navbar agora roda em `backdrop-blur-md` e o Hero foi alinhado ao layout.
- **Cor de Conversão Unificada:** O CTA de "Triagem Inteligente" no Header abandonou o verde-esmeralda inconsistente. Agora ele força a variável **Accent (Laranja Escuro - `#CC5500`)**, garantindo que a cognição de compra principal do site seja sempre 100% laranjada, do desktop ao mobile.
- **Prevenção de Overlap (Safe Padding):** O container flex do Hero (`<main id="hero">`) recebeu as amarras `lg:pt-32` para impedir que ele morda a navbar transparente em telas baixas.

### 2. Acessibilidade Agressiva (WCAG)
- **Focus Trap no Modal:** Era um dos bugs mais graves. A tecla `TAB` agora fica estritamente **enjaulada** dentro do Modal de Triagem quando ele está aberto. Além disso, o atributo `aria-hidden` oculta temporariamente a `<main>` para que leitores de tela não fiquem "andando" no background.
- **Hierarquia de Títulos (Headings):** O site carecia do título H1 e H2 antes do JavaScript agir. Inseri `<h1>` e `<h2>` invisíveis (`sr-only`) interligados por `aria-labelledby` nas seções cruciais, construindo um índice semântico sólido.
- **Semântica Estrutural:** O `<main>` envolvia apenas o Hero. Converti o Hero num `<section>` e criei uma tag mãe `<main id="main-content">` que abraça todo o conteúdo até o Footer.

### 3. Cirurgia no JavaScript Vanilla
- **Morte aos Zumbis:** Variáveis inúteis como `nome`, `whatsapp` e `continuidade` foram evaporadas do estado da `wizardState`. O script agora é focado exclusivamente no roteamento fricção-zero.
- **GPU Accelerated Transitions:** Removi as amarras frágeis de `setTimeout(..., 150)` no crossfade dual funnel. O JavaScript agora escuta o evento real da GPU (`animationend`), eliminando *micro-stutters* na troca de temas. Além disso, adicionei a propriedade `will-change: transform, opacity` no CSS para que o browser reserve memória gráfica pra UI antes da animação acontecer.
- **Retenção de Estado de Volta:** Corrigido o bug visual do Passo 1, onde clicar em "Voltar" no Wizard deixava as opções limpas. O JS agora injeta ativamente um `ring-2` (laranja ou azul) no card que você havia clicado.

---
> [!NOTE]
> Essa bateria blindou a interface contra penalizações do Google Lighthouse (SEO & Acessibilidade) e melhorou o feeling da aplicação em hardwares limitados. A interface agora é *Pro-Max*.
