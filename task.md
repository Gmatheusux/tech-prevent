# <span style="color: #CC5500;">**Workflow Oficial de UX/UI - V6.1 (Visual Validation & Links)**</span>

> [!NOTE]
> Este é o template padrão de operação. O task.md funciona como a **Barra de Progresso Oficial** do projeto, mapeada a partir do Fluxograma inicial. 1 Chat = 1 Fluxo. O agente é proibido de interagir com fluxos fora do escopo do chat atual.
> **Regra Visual:** SEMPRE que o projeto exigir uma aprovação ou validação visual do Gabe (ex: Design System, botões, telas), a IA DEVE gerar e apresentar um arquivo HTML renderizável para validação prática no navegador.

---

## <span style="color: #CC5500;">**FASE 0: Isca Comercial (Prospecção Agressiva)**</span>
> **Responsável:** @researcher | **Modelo:** flash

- [x] Mapear a empresa alvo e invocar subagentes de pesquisa (deep-research).
- [x] Raspar avaliações de usuários (Reclame Aqui, Google Reviews, Ouvidorias).
- [x] Executar **Competitive Audit** (Análise de Competidores) levantando falhas de UX.
- [x] Consolidar o laudo técnico para fechamento comercial. 
- [x] **Obrigatório:** Todos os links de referências, concorrentes e auditorias DEVEM ser formatados como links Markdown clicáveis (ex: [Site](url)) para abertura direta no navegador.

---

## <span style="color: #CC5500;">**A FUNDAÇÃO DO PRODUTO (Feita 1x - Consultada Sob Demanda)**</span>

### <span style="color: #CC5500;">**FASE 1: Arquitetura, UX & Fluxograma (A Bússola)**</span>
> **Responsável:** Gravy | **Modelo:** pro (Gemini 3.1 Pro)

- [x] Definir o escopo completo: Quais telas existirão e o que cada uma fará.
- [x] Gerar um **Fluxograma Visual (Mermaid)** mapeando o User Flow e o Sitemap.
- [x] **Validação Humana:** Gabe aprova o Fluxograma.
- [x] **Atualizar a Barra de Progresso:** Inserir todas as telas aprovadas no task.md e no ActiveContext.md como um checklist.

#### <span style="color: #CC5500;">**Escopo de Telas Aprovado (Checklist de Construção)**</span>
- [ ] Módulo Global: Motor de Triagem Inteligente (Wizard Multi-Step)
- [ ] Tela 1: Home SPA (Hero Switcher B2B/B2C dinâmico)
- [ ] Tela 2: Hub B2C (Metodologia Caixa de Vidro, Bancada, Logística)
- [ ] Tela 3: Hub B2B (Calculadora de Prejuízo, Infra/Racks, Contrato Preventivo)
- [ ] Tela 4: Laboratório Físico & Transparência

### <span style="color: #CC5500;">**FASE 1.5: UX Writing & Copywriting Estratégico (O Tom de Voz)**</span>
> **Responsável:** Gravy | **Modelo:** pro

- [x] Definir a Voz e Tom da Marca (Brand Persona) alinhada à autoridade (B2B) e acessibilidade (B2C).
- [x] Escrever o Copy completo da **Home SPA (Hero, Gatilhos e Switcher)**.
- [x] Escrever o Copy completo do **Hub B2B (Calculadora, Dores, CTAs de Alta Conversão)**.
- [x] Escrever o Copy completo do **Hub B2C (4 Passos Caixa de Vidro, Reparo e Logística)**.
- [x] Escrever o Copy do **Motor de Triagem Inteligente (Perguntas e Respostas do Wizard)**.
- [x] Consolidar todo o texto no arquivo `docs/COPY_DECK.md` para uso estrito nas fases de engenharia.

### <span style="color: #CC5500;">**FASE 2: Design System & O Molde (SSOT)**</span>
- [ ] Mapear variáveis de cor, tipografia e espaçamento via skill ui-ux-pro-max.
- [ ] Gerar Artefato HTML (Style Guide) para validação visual das cores e componentes.
- [ ] Gerar o arquivo raiz DESIGN.md (A Lei Visual) após aprovação do HTML.
- [ ] Extrair lógicas complexas para .agents/rules/ usando YAML Model Decision.
- [ ] Inicializar o repositório Git local. **Encerrar o Chat de Fundação.**

---

## <span style="color: #CC5500;">**O LOOP DE ENGENHARIA (1 Chat = 1 Fluxo Específico)**</span>
> *REGRA DE OURO: O chat atual é bloqueado exclusivamente para o fluxo designado. Proibido interagir com o resto do sistema. Se um fluxo precisar de atualização no futuro, um chat isolado será aberto apenas para ele.*

### <span style="color: #CC5500;">**FASE 3: Engenharia em Contêiner Estrito**</span>
> **Responsável:** @engineer | **Modelo:** pro (Claude Sonnet 4.6)

- [ ] Ler a Barra de Progresso (ActiveContext.md) e focar **apenas** na Tela/Fluxo atual.
- [ ] Iniciar Git Worktree isolada para o desenvolvimento deste fluxo.
- [ ] Codificar em HTML/Tailwind/React ESTRITAMENTE baseado no DESIGN.md e no COPY_DECK.md.
- [ ] Salvar na Worktree e acionar a fase de QA.

### <span style="color: #CC5500;">**FASE 4: QA Visual, Handoff & Merge**</span>
> **Responsável:** @qa e Gabe

- [ ] Subir servidor e acionar Playwright/Chromium para prints/webm da Worktree.
- [ ] Consolidar evidências e HTML renderizável no production_artifacts/walkthrough.md.
- [ ] **PAUSAR (Request Review)**: Gabe faz a aprovação visual no HTML/Vídeo.
- [ ] Gravy comita via Conventional Commits (Regra 17) e faz o merge para main.
- [ ] **Barra de Progresso:** Gravy marca o fluxo com [x] no task.md, atualiza o ActiveContext.md e pergunta qual é o próximo fluxo da lista a ser iniciado em um novo chat.
