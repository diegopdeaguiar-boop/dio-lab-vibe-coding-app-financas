# 💸 App de Finanças Pessoais do Diego Aguiar com Vibe Coding:

PRD refinado com o Copilot Think Deeper:
---
PRD — App de Finanças por Conversa

Visão do produto
Criar um assistente conversacional de finanças pessoais e familiares que permita registrar, classificar e acompanhar receitas, despesas e investimentos em linguagem natural, com recomendações de economia e educação financeira por IA, sem formulários manuais ou planilhas complexas.
Reforço de design: o aplicativo deve adotar um design universal desde o MVP, garantindo acessibilidade, usabilidade e inclusão para o máximo de pessoas possível (ex.: suporte a leitura por voz, navegação por teclado, alto contraste, tipografia legível, textos alternativos, fluxos simplificados e linguagem clara).

Resumo executivo
Problema: dificuldade de famílias e indivíduos em controlar finanças; tabus sobre finanças familiares; baixa adesão a hábitos de investimento.
Solução: app conversacional com visão pessoal e familiar em uma única conta, classificação automática de transações, metas, recomendações do “Agente Financeiro” e visualizações simples.
Público‑alvo: iniciantes em organização financeira e famílias que buscam praticidade.

Objetivos e métricas de sucesso
- Aumentar a adesão: 30% dos usuários ativos registrando transações via chat nas primeiras 2 semanas.
- Precisão de classificação: ≥85% de acerto automático nas categorias de transação no MVP.
- Engajamento com metas: 25% dos usuários criando ao menos 1 meta financeira no primeiro mês.
- Retenção: 40% de retenção mensal após 30 dias.

Requisitos principais (MVP)

Funcionais (prioridade alta)
1. Registro por chat em linguagem natural — usuário informa receitas, despesas e investimentos conversando.
2. Classificação automática de transações — categorias padrão e possibilidade de correção manual.
3. Visão Pessoal e Familiar — alternância/combinação de visões dentro da mesma conta.
4. Metas financeiras — criar, acompanhar progresso e receber lembretes.
5. Agente Financeiro — dicas de economia, alertas de despesas críticas e recomendações de organização.
6. Investimentos — item específico com classificação: renda fixa; renda variável; reserva de emergência; juros/proventos/dividendos.
7. Relatórios e gráficos simples — receitas vs despesas, composição de gastos, evolução de investimentos.
8. Tela inicial com quadro de dicas — recomendações dinâmicas e alertas de despesas críticas com impacto percentual sobre receita e despesa total.

Não funcionais (prioridade média)
- Design universal e acessível (contraste, leitura, navegação por voz, suporte a leitores de tela, controles ampliáveis, linguagem simples).
- Privacidade e segurança: criptografia de dados sensíveis e consentimento claro para uso de IA.
- Performance: resposta do chat < 2s para interações básicas.

Regras de negócio e comportamentos da IA
- Ao identificar despesa crítica, o app deve:
  - notificar o usuário;
  - mostrar impacto percentual sobre receita total e despesa total;
  - sugerir 2–3 ações práticas para reduzir ou reorganizar essa despesa.
- Classificação de investimentos deve aceitar entradas manuais e reconhecer termos comuns (ex.: "CDB", "ações", "dividendos").
- Separar automaticamente entradas de proventos/juros/dividendos e vinculá‑las ao ativo correspondente.

Principais telas do MVP

Tela | Objetivo | Elementos-chave
Home | Visão rápida e dicas; alertas | Quadro de dicas; resumo receita/despesa; alertas de despesa crítica
Chat / Registro | Registrar transações por conversa | Campo de chat; histórico; botões rápidos (receita, despesa, investimento)
Transações | Listar e editar lançamentos | Lista filtrável; categoria; editar/confirmar classificação
Investimentos | Gerenciar carteira | Lista de ativos; classificação (renda fixa/variável/reserva); proventos
Metas | Criar e acompanhar metas | Meta, prazo, progresso, sugestões de aporte
Relatórios | Visualizar gráficos simples | Gráficos: pizza, linha, barras; período selecionável

Fluxo de interação essencial (MVP)
1. Onboarding curto: pedir visão (pessoal/familiar), metas iniciais e permissão para analisar transações.
2. Registro por chat: usuário digita "Gastei R$ 50 no mercado" → IA extrai valor, categoria provável, data e confirma.
3. Classificação automática: IA sugere categoria; usuário confirma ou corrige.
4. Alerta de despesa crítica: IA detecta gasto recorrente alto → mostra impacto percentual e recomenda ação.
5. Investimentos: usuário registra aporte; IA classifica e atualiza gráfico de carteira.

Requisitos técnicos e recursos necessários
- Backend: API para conversação, processamento de linguagem natural (NLP), motor de regras para classificação e cálculo de métricas.
- Modelos IA: NLU para extração de entidades (valor, categoria, data, tipo de investimento); modelo de classificação de transações; mecanismo de recomendação simples.
- Banco de dados: estrutura para contas, membros da família, transações, ativos e metas.
- Frontend: app mobile (iOS/Android) com componente de chat e dashboards leves.
- Design: kit de UI acessível e responsivo com foco em legibilidade e princípios de design universal (contraste, escalabilidade de fonte, navegação por teclado, compatibilidade com leitores de tela, linguagem simples).
- Segurança: autenticação, criptografia em trânsito e repouso, políticas de consentimento.

Plano de MVP e esboço de validação inicial

Fase 0 — Preparação (2 semanas)
- Definir personas e jornada do usuário.
- Mapear intents e entidades para o chat.
- Criar protótipos de baixa fidelidade das telas principais.

Fase 1 — Construção do MVP (8–10 semanas)
- Implementar chat básico com NLU para registrar receitas/despesas/investimentos.
- Implementar classificação automática com regras + ML simples.
- Desenvolver telas Home, Chat, Transações, Investimentos, Metas e Relatórios.
- Implementar quadro de dicas e lógica de despesa crítica.

Fase 2 — Testes e validação (3–4 semanas)
- Teste com 20–50 usuários reais do público‑alvo.
- Métricas de validação: taxa de registro via chat, precisão de classificação, criação de metas, feedback de usabilidade.
- Coletar correções de linguagem, categorias faltantes e pontos de fricção no fluxo familiar.

Fase 3 — Iteração (4 semanas)
- Ajustar NLU e categorias com dados reais.
- Melhorar UX do fluxo familiar e visualizações.
- Preparar roadmap para integrações bancárias e automações futuras.

Critérios de aceitação do MVP
- Registro por chat funcionando para entradas comuns com confirmação do usuário.
- Classificação automática com precisão ≥85% em amostra de validação.
- Tela Home com quadro de dicas e alerta de despesa crítica mostrando impacto percentual.
- Item de investimentos com classificação mínima e registro de proventos.
- Relatórios básicos com gráficos interativos.
- Critério de acessibilidade: checklist de design universal aplicado (ex.: conformidade com padrões de contraste, navegação por teclado, textos alternativos, suporte a leitores de tela) e validação com pelo menos 5 usuários com necessidades de acessibilidade.

Riscos e mitigação (resumo)
- NLU imprecisa → mitigar com regras híbridas e revisão humana inicial.
- Privacidade → mitigar com consentimento explícito e criptografia.
- Adoção familiar baixa → mitigar com onboarding orientado e exemplos práticos.
- Acessibilidade negligenciada → mitigar incluindo testes com usuários reais com diferentes necessidades e aplicando checklist de design universal desde o início.

Síntese didática: O que é um PRD
Um PRD (Product Requirements Document) é um documento que descreve a visão, objetivos, público, funcionalidades e critérios de sucesso de um produto, servindo como ponte entre estratégia e execução para equipes multifuncionais. PRDs modernos são documentos vivos, focados em necessidades do usuário e em requisitos acionáveis para desenvolvimento ágil.

Síntese didática: O que é vibe coding
Vibe coding é uma abordagem prática e iterativa para criar produtos e artefatos (PRDs, protótipos, prompts) com foco em velocidade e experimentação. Envolve usar templates, prompts e ciclos rápidos de feedback para transformar ideias em protótipos funcionais, priorizando entrega de valor mínimo viável e refinamento contínuo.

Observação final
O design universal foi incluído explicitamente na visão, requisitos não funcionais, design e critérios de aceitação. Pode-se complementar este PRD com um checklist de acessibilidade para o sprint 0.


---

## Interações com o Lovable:
> Crie um app de finanças pessoas, com base no seguinte PRD (Product Requirements Document):
> Escopo inicial: MVP Completo; Design: Vibrante e Amigável; Visão Familiar: Apenas alternância de visão; Autenticação: Sim, com email/senha
> Plan approved.

## Resultado Final no Lovable:
<img width="1857" height="908" alt="image" src="https://github.com/user-attachments/assets/f237a499-d6fd-4987-b768-3ee1ca8b9b98" />

<img width="1877" height="916" alt="image" src="https://github.com/user-attachments/assets/7f6e9f51-9609-4e3b-956d-11c63cb7bfc8" />

## Resumo do app
Resumo do app (baseado na foto)

Nome: FinançaChat
Visão: assistente conversacional para controle financeiro pessoal.

Visão atual exibida: Visão pessoal • fevereiro de 2026

Resumo financeiro
- Receitas: R$ 6.100,00
- Despesas: R$ 1.699,99
- Saldo: R$ 4.400,01

Ações rápidas
- Registrar via chat
- Ver lista de transações
- Acessar carteira de investimentos
- Acessar metas/objetivos

Destaques do Agente Financeiro
- Alerta de despesa: alimentação representa 25% da receita; sugestão de planejar refeições; mostra impacto percentual.
- Reserva de emergência: 51% acumulado; incentivo a continuar aportes.

Navegação principal
- Home, Chat, Transações, Investimentos, Metas, Relatórios

Observações funcionais implícitas
- Interface centrada em conversação para registrar entradas financeiras.
- Painel inicial com resumo rápido e dicas acionáveis.
- Seções para transações, investimentos e metas, com navegação por abas.
- Indicadores de impacto percentual e mensagens do agente para orientar o usuário.
  
## Reflexão sobre o processo
### O que funcionou bem?  
A dica do professor em refinar no Copilot ajudou muito, pois os crédito so Lavable são poucos.

### O que não funcionou como o esperado?  
Consumi todos os créditos antes de concluir o app.

### O que aprendeu sobre conversar com IAs?
Aprendi que preciso ser bem detalhista e claro o suficiente no que desejo na interação.
