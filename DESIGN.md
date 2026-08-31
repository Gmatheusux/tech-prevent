---
brand_name: "Tech Prevent"
version: "1.0.0"
status: "Fase 2 - Fundação UI Aprovada"

typography:
  headings: "Poppins, sans-serif"
  body: "Open Sans, sans-serif"
  weights:
    regular: 400
    bold: 700
    black: 900

colors:
  primary: "#1A4E66"     # Azul Petróleo (Cor Exata do Escudo/Logo original)
  primaryDark: "#0D2D3D"
  secondary: "#3B82F6"
  accent: "#CC5500"      # Laranja de Conversão e Destaque
  accentDark: "#A34300"
  surface: "#F8FAFC"

ui_tokens:
  glassmorphism:
    nav_scrolled_bg: "rgba(0, 0, 0, 0.6)"
    nav_scrolled_blur: "12px"
    nav_border: "rgba(255, 255, 255, 0.1)"
    hero_card_bg: "rgba(15, 23, 42, 0.4)" # slate-900/40
    hero_card_blur: "24px"
    hero_card_shadow: "0 8px 32px rgba(0,0,0,0.5)"
  
  images:
    logo_dark_mode: "brightness(0) invert(1)" # Transforma logo escura em branca absoluta
---

# Design System & UI Architecture (Tech Prevent)

Este arquivo é a "Lei Visual" (Single Source of Truth) para todo o desenvolvimento Front-end do portal Tech Prevent. Quaisquer novas páginas ou seções devem herdar as variáveis técnicas do cabeçalho YAML acima.

## 1. O Paradigma de Navegação (Dual Funnel)
O site atua como um ecossistema SPA (Single Page Application) onde a decisão da "Persona" ocorre imediatamente no topo da página.

- **Componente Core:** O `Toggle Pill` (Segmented Control).
- **Regra de Negócio:** O site é renderizado sempre focando em **B2C (Uso Pessoal)** como estado inicial `onLoad`. O estado **B2B (Empresas)** é invocado via clique do usuário no Toggle, executando transições crossfade, substituindo background e copywriting na mesma tela, sem reload.

## 2. A Navbar (Dynamic Morphing)
A barra de navegação global ignora botões de login (O escopo é 100% Institucional/Geração de Leads).

- **Estado Topo (Y=0):** Totalmente invisível. Fundo transparente, sem bordas, alto padding (`py-6`), permitindo imersão total na fotografia da Hero.
- **Estado Scrolled (Y>20):** Acionamento do Glassmorphism pesado (padrão Vercel/Apple). Fundo preto translúcido, desfoque de vidro, retração de padding (`py-3`) e borda inferior sutil de 10% de opacidade branca (`border-white/10`).

## 3. A Hero (Glassmorphism Card)
O núcleo do conteúdo não repousa diretamente sobre imagens intensas.
Ele é encapsulado em um componente Flutuante de Vidro (Card Glassmorphism), garantindo um nível brutal de legibilidade para o H1 e CTAs, isolando o ruído fotográfico. 

- **A Fotografia de Fundo:** Só podem ser utilizadas imagens *Hiper-Realistas* que remetam ao conceito de "Caixa de Vidro" e Transparência. (Equipamento claro, limpo, iluminado cinematicamente). Não utilizar bancos genéricos irreais.
- **Copywriting:** Utilizar sempre uma Label Tag (Pílula superior de contexto, ex: "Uso Pessoal"), seguida de um H1 dramático (`font-black`), parágrafo conciso focado na dor, e botão primário com ícone.

## 4. Componentes Interativos CSS
Para simular as animações orgânicas utilizadas no protótipo `index.html`:
- Utilizar a classe `fade-in` (`translateY` + `opacity`) com `0.5s cubic-bezier(0.4, 0, 0.2, 1)`.
- Evitar display block/none duros. Realizar fading out (opacity 0) antes da troca de nós no DOM para transições perfeitas do Dual Funnel.
