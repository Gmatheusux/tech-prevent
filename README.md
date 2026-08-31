# Tech Prevent - Landing Page & Motor de Triagem Inteligente

Bem-vindo ao repositório oficial da **Tech Prevent**. Este projeto foi desenvolvido visando alta performance, zero fricção de conversão e um design system ancorado em *Glassmorphism* e dual-tone (B2B/B2C).

## 🚀 O Projeto

A Tech Prevent é uma empresa de suporte e gestão de TI no Rio de Janeiro. A solução desenvolvida consiste em:
1. **Landing Page Dual-Funnel (SPA):** Transição morfológica acelerada por GPU que altera todo o conteúdo, paleta e copys dependendo da modalidade de uso do usuário (Para Você / Para Empresas).
2. **Motor de Triagem Inteligente:** Um Wizard multi-step modal com *Focus Trap* (Acessibilidade WCAG) que coleta os dados do usuário e envia um payload codificado diretamente para o WhatsApp oficial, sem necessidade de banco de dados ou formulários pesados.

## 📁 Estrutura de Documentação (Cofre)

O projeto adota a arquitetura de duplo nível e documentação isolada. Todos os padrões visuais e comportamentais estão documentados nos arquivos listados abaixo:

- [`DESIGN.md`](./DESIGN.md): **(Core)** Central de Tokens de Design. Contém as regras de tipografia (Inter/Montserrat), paleta de cores (`#1A4E66` e `#CC5500`), regras de Glassmorphism e restrições de UI/UX.
- [`ActiveContext.md`](./ActiveContext.md): **(Memória)** Rastreador de estado atual do projeto, próximas pendências e log de handoffs.
- [`docs/COPY_DECK.md`](./docs/COPY_DECK.md): Estrutura oficial de *copywriting*, gatilhos mentais e conteúdo textual.
- [`docs/QA_AUDIT_HANDOFF.md`](./docs/QA_AUDIT_HANDOFF.md): Registro das auditorias de acessibilidade (WCAG), limpeza de código JS e refinamento de interface aplicadas antes da entrega final.

## 🛠 Stack Tecnológica

- **HTML5 Semântico:** Estruturado sob rígidas regras da WCAG (Navegação por teclado, *Focus Rings*, Aria Labels, Headings lógicos).
- **Tailwind CSS (CDN):** Estilização utilitária de ponta a ponta com preflights customizados.
- **JavaScript Vanilla (ES6):** Gestão de estado global (`wizardState`), transições de classe baseadas em `animationend` (GPU-first) e injeção de DOM.
- **Design:** Glassmorphism fluido, blur-drops calculados e sombras projetadas (*glow*).

## 💻 Como Rodar Localmente

O projeto não requer Node modules volumosos para build final. Basta servir o arquivo estático na raiz:

```bash
# Iniciar servidor local
npx http-server . -p 8080 -c-1
```
Abra `http://localhost:8080` em seu navegador.

## 🔐 Compliance e Regras

- **Zero Trust UI:** Qualquer nova seção deve herdar os tokens estritos do `DESIGN.md`.
- **Acessibilidade Inegociável:** Novos modais exigem *Focus Trap*. Novos botões exigem `focus-visible`.
- **Commits:** Histórico versionado com *Conventional Commits* garantindo auditoria clara.

---
*Engenharia UI/UX orquestrada pela arquitetura Antigravity.*
