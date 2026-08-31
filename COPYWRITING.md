# COPYWRITING (TECH PREVENT)

Este documento é a Fonte da Verdade (SSOT) para toda a redação, tom de voz e interface textual do portal da Tech Prevent (B2B e B2C).

---

## 1. DIRETRIZES DE VOZ E TOM

### Tom de Voz da Marca
- **Empático e Acolhedor:** O cliente quase sempre nos procura num momento de imprevisto e estresse (falha técnica, sistema fora do ar, computador quebrado). A comunicação não deve amplificar o pânico, mas sim agir como um "porto seguro". 
- **Consultivo e Transparente:** Explicamos a tecnologia de forma acessível. O usuário deve sentir que somos parceiros confiáveis, não apenas prestadores de serviço mecânicos.
- **Autoridade sem Arrogância:** Demonstramos nossa infraestrutura (Laboratório Físico, Service Desk) através de processos claros (Metodologia Caixa de Vidro).

### Vocabulário-chave
- Tranquilidade, Estabilidade, Parceria, Transparência, Produtividade, Prevenção, Segurança, Acolhimento, Etapas Claras, Conforto.

### Termos Proibidos (O que NÃO dizer)
- **Marketing de Terror/Medo:** "Você vai perder dinheiro", "Prejuízo enorme", "Sua TI é uma bomba-relógio". (Pivotamos para focar no tempo/produtividade ganha).
- **Jargões Técnicos Vazios:** Evitar siglas que assustem o cliente B2C ou o gestor B2B sem formação técnica.
- **Falsa Urgência:** "Compre agora antes que piore", "Última chance".

---

## 2. ESPECIFICAÇÃO DE COPY POR SEÇÃO

### A. SEÇÃO: HERO (HOME SPA - SWITCHER DINÂMICO)
*A interface muda dependendo se o usuário seleciona Empresa (B2B) ou Pessoal (B2C).*

#### Estado B2B (Empresas)
- **Eyebrow (Tagline):** Para Minha Empresa
- **Headline Principal (H1):** TI Corporativa com Escalabilidade e Segurança para o seu Negócio.
- **Subheadline:** Da infraestrutura de redes ao Service Desk completo. Prevenimos problemas antes que eles parem a sua operação.
- **Botão Primário:** Realize sua cotação
- **Botão Secundário:** Falar com um Especialista
- **Microcopys (Badges de Confiança):** 
  - Gestão de Ativos & Segurança de Dados
  - Suporte Preventivo N1, N2 e N3

#### Estado B2C (Pessoa Física)
- **Eyebrow (Tagline):** Para Meu Uso Pessoal
- **Headline Principal (H1):** Reparo de Computadores com 100% de Transparência.
- **Subheadline:** Conheça a metodologia "Caixa de Vidro". Acompanhe cada etapa do conserto do seu equipamento, via whatsapp.
- **Botão Primário:** Solicitar Diagnóstico Agora
- **Botão Secundário:** Como funciona o Reparo?
- **Microcopys (Badges de Confiança):** 
  - Laboratório Físico Avançado no RJ
  - Sistema Leva & Traz Exclusivo

---

### B. SEÇÃO: FEATURES B2B (ESTABILIDADE E PRODUTIVIDADE)
- **Eyebrow:** Soluções Corporativas
- **Headline Principal (H2):** A base silenciosa para o crescimento do seu negócio.
- **Subheadline:** Sabemos que a melhor TI é aquela que você não precisa lembrar que existe, porque tudo simplesmente funciona. Garantimos a estabilidade da sua operação.
- **Botão Primário:** Agendar um Bate-Papo Consultivo
- **Microcopys (Cards de Serviço):**
  - **Service Desk Acolhedor:** Atendimento ágil e paciente.
  - **Gestão Preventiva:** Prevenção antes de apagar incêndios.
  - **Segurança e Organização:** Proteção do seu bem mais valioso: a informação.

---

### C. SEÇÃO: FEATURES B2C (CAIXA DE VIDRO E LOGÍSTICA)
- **Eyebrow:** Reparo Seguro
- **Headline Principal (H2):** Cuidamos do seu equipamento com o respeito que você merece.
- **Subheadline:** Quando o imprevisto acontece, você precisa de clareza e de alguém em quem confiar. Acompanhe cada etapa, de ponta a ponta.
- **Botão Primário:** Solicitar Atendimento
- **Microcopys (Os 4 Passos):**
  1. Check-in Cuidadoso
  2. Diagnóstico Claro (Visual via foto/vídeo)
  3. Reparo Acompanhado (Atualizações via WhatsApp)
  4. Testes de Qualidade

---

### D. SEÇÃO: MOTOR DE TRIAGEM INTELIGENTE (WIZARD & CTA FINAL)
- **Eyebrow:** Como podemos ajudar?
- **Headline Principal (H2):** Para podermos direcionar o especialista ideal, você busca ajuda para:
- **Subheadline:** Responda 3 perguntas rápidas para agilizarmos seu atendimento.
- **Botão Primário (Final):** Iniciar Atendimento via WhatsApp
- **Microcopys de Seleção B2C:** 
  - Qual o equipamento? "Notebook", "Computador de Mesa (Desktop)", "PC Gamer", "Outro".
  - Logística: "Levar ao laboratório", "Preciso do Leva & Traz", "Tirar dúvidas".

---

## 3. VALIDAÇÃO DE ACESSIBILIDADE E UX

- **Clareza de Ação (Aria Labels & Calls to Action):**
  - Não existem botões genéricos (como "Clique aqui" ou "Saiba mais").
  - Botões utilizam verbos de ação focados em resultado: `Realize sua cotação`, `Solicitar Diagnóstico Agora`, `Iniciar Atendimento via WhatsApp`.
- **Estados de Formulário (Inputs do Wizard):**
  - **Label:** `Como podemos te chamar?` em vez do mecânico `Nome Completo`.
  - **Label:** `Qual o seu WhatsApp?` em vez do obsoleto `Telefone Fixo / Celular`.
- **Estados de Loading/Erro:**
  - **Loading:** "Iniciando seu atendimento..." ou "Preparando link direto para o WhatsApp..."
  - **Erro Form:** "Por favor, preencha o seu nome para sabermos como falar com você." (Foco amigável e explicativo).
- **Leitores de Tela:**
  - Badges de prova social (ex: ícones de segurança) devem conter atributos textuais clarificando que a Tech Prevent possui laboratório físico no RJ e sistemas estruturados.
