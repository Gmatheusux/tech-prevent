# Active Context

## Atualizações Recentes (Fase 1 Encerrada)
- **Arquitetura de Duplo Funil (B2B vs B2C)** definida e aprovada.
- **Ecossistema SPA:** A Home atuará com um Switcher Global (estado) para alterar instantaneamente todo o contexto (textos, CTAs, dores) dependendo da persona escolhida.
- **Gatilhos de UX e Ferramentas Interativas:**
  - B2B: Foco em redução de risco financeiro, segurança e estabilidade (Prevenção e Service Desk).
  - B2C: Implementação da Metodologia "Caixa de Vidro" (4 passos para combater o medo de extorsão) e roteamento de logística segura.
- **Motor de Triagem Inteligente:** Um Wizard multi-step global substitui o contato passivo genérico.
- O mapeamento visual e as decisões foram registradas.

## Escopo de Telas / Fluxos Aprovados
- [ ] **Módulo Global:** Motor de Triagem Inteligente (Wizard Multi-Step)
- [ ] **Tela 1:** Home SPA (Hero Switcher B2B/B2C dinâmico)
- [ ] **Tela 2:** Hub B2C (Metodologia Caixa de Vidro, Bancada, Logística)
- [ ] **Tela 3:** Hub B2B (Soluções Corporativas, Infra/Racks, Contrato Preventivo)
- [ ] **Tela 4:** Laboratório Físico & Transparência Técnica

## Decisões Estratégicas & Negócio Consolidadas
- **Posicionamento:** Site 100% Institucional & Focado em Autoridade/Conversão de Serviços de TI no RJ.
- **Atendimento B2C:** Laboratório próprio (balcão), serviço Leva & Traz (coleta/delivery no RJ) e visitas residenciais.
- **Engenharia de Hardware:** Manutenção avançada de notebooks/desktops, montagem de computadores custom com consultoria e fornecimento de peças em bancada.
- **Gestão B2B:** Full Service Desk, rotinas preventivas com inventário de ativos, projetos de cabeamento/racks e firewalls corporativos.
- **UX Core:** Switcher B2B vs B2C na Hero, Jornada Transparente em 4 Passos e CTAs inteligentes no WhatsApp.

## Atualizações Recentes (Fase 1.5 Encerrada)
- **Tom de Voz e Brand Persona:** Abordagem empática, consultiva e humana. Foco em qualidade, estabilidade (B2B) e acolhimento transparente (B2C), fugindo do tom agressivo/desesperado.
- **Copying Finalizado:** Textos da Home, Hub B2B, Hub B2C e Motor de Triagem Inteligente foram consolidados no arquivo `docs/COPY_DECK.md`.
- O Motor de Triagem separa explicitamente Desktop de PC Gamer para um roteamento mais preciso no B2C.

## Atualizações Recentes (Fase 3: Validação Completa & QA Aprovado)
- **Otimização de Assets WebP:** Todas as imagens (`b2c_img.webp`, `b2b_img.webp`, `logo1.webp`, `logo2.webp`) convertidas com redução de até 83.9% no payload.
- **Hero Fluida & Switcher Dual Funnel Validado:**
  - Segmented Control com Glider deslizante via aceleração de hardware GPU (`translate3d`) e curva `cubic-bezier(0.16, 1, 0.3, 1)`.
  - Micro-interações táteis nos botões (efeito shimmer passante, elevação no hover e active press feedback).
  - Navbar com dynamic morphing glassmorphism no scroll e botão de CTA ajustado para "WhatsApp".
- **Refinamentos de Acessibilidade e UX Aplicados:**
  - Preservação dos anéis de foco acessível (`focus-visible:ring-2`) em todas as transições via teclado.
  - Links externos para o WhatsApp no CTA secundário agora abrem corretamente com `target="_blank" rel="noopener noreferrer"`.
  - Controle de estado `aria-expanded` dinâmico no menu mobile.
  - Ícones SVG decorativos com `aria-hidden="true"`.
- **Servidor Localhost Ativo:** Projeto rodando e 100% validado na porta `8080`.

## Próxima Etapa Pendente (Fase 4)
- **FASE 4: Construção do Hub B2C (Metodologia Caixa de Vidro) e Hub B2B (Soluções Corporativas)**
  - Implementar as seções detalhadas de serviço abaixo da Hero.
  - Implementar o Motor de Triagem Inteligente (Wizard Multi-Step) com roteamento para WhatsApp.


