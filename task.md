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
- [x] Tela 1: Home SPA (Hero Switcher B2B/B2C dinâmico) — **Concluído na Fase 3**
- [ ] Tela 2: Hub B2C (Metodologia Caixa de Vidro, Bancada, Logística)
- [ ] Tela 3: Hub B2B (Soluções Corporativas, Infra/Racks, Contrato Preventivo)
- [ ] Tela 4: Laboratório Físico & Transparência

### <span style="color: #CC5500;">**FASE 1.5: UX Writing & Copywriting Estratégico (O Tom de Voz)**</span>
> **Responsável:** Gravy | **Modelo:** pro

- [x] Definir a Voz e Tom da Marca (Brand Persona) alinhada à autoridade (B2B) e acessibilidade (B2C).
- [x] Escrever o Copy completo da **Home SPA (Hero, Gatilhos e Switcher)**.
- [x] Escrever o Copy completo do **Hub B2B (Soluções, Dores, CTAs de Alta Conversão)**.
- [x] Escrever o Copy completo do **Hub B2C (4 Passos Caixa de Vidro, Reparo e Logística)**.
- [x] Escrever o Copy do **Motor de Triagem Inteligente (Perguntas e Respostas do Wizard)**.
- [x] Consolidar todo o texto no arquivo `docs/COPY_DECK.md` para uso estrito nas fases de engenharia.

### <span style="color: #CC5500;">**FASE 2: Design System & O Molde (SSOT)**</span>
- [x] Mapear variáveis de cor, tipografia e espaçamento via skill ui-ux-pro-max.
- [x] Gerar Artefato HTML (Style Guide) para validação visual das cores e componentes.
- [x] Gerar o arquivo raiz DESIGN.md (A Lei Visual) após aprovação do HTML.
- [x] Inicializar o repositório Git local. **Encerrar o Chat de Fundação.**

---

## <span style="color: #CC5500;">**O LOOP DE ENGENHARIA (1 Chat = 1 Fluxo Específico)**</span>

### <span style="color: #CC5500;">**FASE 3: Engenharia da Hero & Switcher Dual Funnel**</span>
> **Responsável:** Gravy / @engineer | **Status:** ✅ Concluído e Validado

- [x] Otimização de Assets (Conversão de JPG/PNG para WebP com até 83.9% de redução).
- [x] Construção da Navbar Dynamic Morphing Glassmorphism com CTA "WhatsApp".
- [x] Implementação do Segmented Control com Glider acelerado por hardware GPU (`translate3d`).
- [x] Implementação do Switcher Dual Funnel (B2C e B2B) com tokens do `DESIGN.md` e redação do `COPY_DECK.md`.
- [x] Auditoria de Acessibilidade WCAG 2.2 (Preservação de `focus-visible`, `aria-expanded` no mobile, `aria-hidden` em SVGs).
- [x] Validação e Servidor Localhost ativo na porta 8080.
- [x] Commits semânticos no Git e handoff para o próximo contêiner.

---

## <span style="color: #CC5500;">**PRÓXIMA SESSÃO (Novo Chat / Contêiner Isolado)**</span>

### <span style="color: #CC5500;">**FASE 4: Construção dos Hubs de Serviços & Motor de Triagem**</span>
- [ ] **Fluxo 1:** Seção Hub B2C (Metodologia Caixa de Vidro em 4 Passos, Bancada e Sistema Leva & Traz).
- [ ] **Fluxo 2:** Seção Hub B2B (Soluções Corporativas, Service Desk, Infra/Racks e Segurança de TI).
- [ ] **Fluxo 3:** Motor de Triagem Inteligente (Wizard Multi-Step com roteamento dinâmico para WhatsApp).
