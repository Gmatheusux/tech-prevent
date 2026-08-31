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

## Próxima Etapa Pendente (Novo Chat — Fase 2)
- **FASE 2: Design System & O Molde (SSOT)**
  - O próximo chat (nova aba) assumirá a construção do Design System.
  - **Diretriz Pré-aprovada para a Fase 2:** Utilizar o padrão "Trust & Authority" (Flat Design).
  - **Cores Sugeridas:** Primária (#1E40AF - Azul Corporativo), Secundária (#3B82F6), Ação (#CC5500 - Laranja), Background (#F8FAFC), Foreground (#0F172A).
  - **Tipografia:** Poppins (Headings) e Open Sans (Body).
  - **Tarefas do próximo agente:**
    1. Gerar o Artefato HTML (Style Guide) com essas variáveis para validação visual.
    2. Após validação, gerar o arquivo raiz `DESIGN.md`.
    3. Extrair lógicas complexas para `.agents/rules/` e inicializar o repositório Git local. Encerrar o ciclo de fundação.
