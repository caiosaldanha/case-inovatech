# Prompts Utilizados (Framework P.R.O.M.P.T)

Ferramenta usada: Claude (Anthropic). Todos os prompts abaixo seguem o framework **P.R.O.M.P.T** (Papel, Restrições, Objetivo, Moldura, Panorama, Tom e Testes) ensinado no caderno da disciplina, e foram usados para gerar os itens 1 a 4 do desafio de consultoria PMO da InovaTech (o item 5 — relatório de impacto/ROI do PMO em 12 meses — foi deliberadamente excluído do escopo).

---

## Prompt 1 — Diagnóstico do PMO e escolha do modelo

- **Papel:** Aja como um consultor sênior de PMO (Project Management Office), especialista em turnaround de portfólio de TI.
- **Restrições:** Não sugira demissões ou corte de equipe; não recomende um modelo de PMO sem justificar com base no cenário de crise descrito; não ignore a urgência financeira do CEO.
- **Objetivo:** Diagnosticar por que a InovaTech precisa de um PMO agora e recomendar qual modelo — Suporte, Controle ou Diretivo — deve ser adotado, com justificativa.
- **Moldura:** Responda em até 6 bullets: 3 para o diagnóstico (causas-raiz) e 3 para a justificativa do modelo escolhido, seguido de uma frase sobre evolução do modelo ao longo do tempo.
- **Panorama:** A empresa é a InovaTech (estudo de caso): silos entre Comercial, Marketing e Tecnologia; 8 projetos ativos sem critério de priorização; retrabalho de 30% do tempo dos devs; visibilidade zero para o CEO; conselho vendo a empresa como "caixa preta".
- **Tom e Testes:** Tom direto e executivo, sem jargão técnico de metodologia ágil; use os números do caso (retrabalho, churn, orçamento parado) como evidência.

**Prompt final aplicado:**
> "Aja como um consultor sênior de PMO especialista em turnaround de portfólio de TI (Papel). Não sugira demissões ou corte de equipe, e não recomende um modelo sem justificar com o cenário descrito (Restrições). Diagnostique por que a InovaTech precisa de um PMO agora e recomende qual modelo — Suporte, Controle ou Diretivo — deve ser adotado (Objetivo). Responda em até 6 bullets: 3 de diagnóstico e 3 de justificativa do modelo, mais uma frase sobre evolução do modelo no tempo (Moldura). A empresa é a InovaTech: silos entre Comercial/Marketing/Tecnologia, 8 projetos sem priorização, 30% do tempo dos devs em retrabalho, visibilidade zero para o CEO, conselho vendo a empresa como 'caixa preta' (Panorama). Tom direto e executivo, sem jargão de metodologia ágil, usando os números do caso como evidência (Tom e Testes)."

---

## Prompt 2 — Quick Wins de curto prazo

- **Papel:** Aja como um gerente de PMO recém-contratado no primeiro mês de mandato.
- **Restrições:** As ações não podem exigir orçamento adicional nem mais de 30 dias para implementar; não proponha nenhuma ferramenta paga nova.
- **Objetivo:** Listar 3 ações práticas de curto prazo que dão visibilidade real aos projetos e organizam a comunicação entre as áreas.
- **Moldura:** Formato de lista numerada (1 a 3), cada item com no máximo 2 linhas: o quê fazer + qual problema específico do case ele resolve.
- **Panorama:** Mesmo panorama de silos e falta de comunicação entre Comercial, Marketing e Tecnologia da InovaTech; relatórios de status hoje são subjetivos e conflitantes.
- **Tom e Testes:** Tom pragmático, orientado a ação imediata — nada de "criar uma cultura de X"; peça ações concretas e verificáveis em 30 dias.

**Prompt final aplicado:**
> "Aja como um gerente de PMO no primeiro mês de mandato (Papel). As ações não podem exigir orçamento adicional nem mais de 30 dias para implementar, e não proponha ferramentas pagas novas (Restrições). Liste 3 ações práticas de curto prazo que dão visibilidade real aos projetos e organizam a comunicação entre as áreas (Objetivo). Formato de lista numerada, cada item com no máximo 2 linhas: o que fazer + qual problema do case resolve (Moldura). A InovaTech tem silos entre Comercial, Marketing e Tecnologia, e relatórios de status hoje são subjetivos e conflitantes (Panorama). Tom pragmático e orientado a ação imediata, sem frases genéricas de 'mudança de cultura' (Tom e Testes)."

---

## Prompt 3 — Critérios de priorização (pesos por ROI, Alinhamento, Urgência e Risco)

- **Papel:** Aja como um analista de estratégia e portfólio, responsável por transformar Missão, Visão e Valores em critérios objetivos de decisão.
- **Restrições:** Os pesos de ROI, Alinhamento Estratégico, Urgência e Risco devem somar 100%; não proponha mais de 4 critérios; não use critérios subjetivos sem ligação com a Missão/Visão/Valores fornecidos.
- **Objetivo:** Definir pesos (%) para ROI, Alinhamento Estratégico, Urgência e Risco, com uma justificativa de 1 linha por critério, ligando o peso à Missão/Visão/Valores e ao momento de crise financeira da empresa.
- **Moldura:** Tabela com colunas Critério | Peso | Justificativa (1 linha).
- **Panorama:** Missão foca em transformar dados em valor real; Visão foca em ser referência em inovação nas Américas; Valores incluem inovação contínua, foco no cliente, crescimento/adaptação e colaboração/excelência. O CEO quer resultados no balanço financeiro, não só gráficos.
- **Tom e Testes:** Tom analítico e defensável perante o board; os pesos devem refletir que é um momento de crise de caixa (ROI e Urgência não podem ser triviais), sem abandonar o Alinhamento Estratégico ao Projeto Phoenix.

**Prompt final aplicado:**
> "Aja como um analista de estratégia e portfólio (Papel). Os pesos de ROI, Alinhamento Estratégico, Urgência e Risco devem somar 100%, sem mais de 4 critérios e sem critérios desconectados da Missão/Visão/Valores (Restrições). Defina o peso de cada critério com justificativa de 1 linha ligando-o à Missão/Visão/Valores e ao momento de crise financeira (Objetivo). Formato de tabela: Critério | Peso | Justificativa (Moldura). Missão: transformar dados em valor real para os clientes; Visão: ser referência em inovação nas Américas; Valores: inovação contínua, foco no cliente, crescimento/adaptação, colaboração/excelência; o CEO quer resultado no balanço financeiro, não só gráficos (Panorama). Tom analítico e defensável perante o board, refletindo que é um momento de crise de caixa (Tom e Testes)."

---

## Prompt 4 — Saneamento de portfólio (cancelar x acelerar)

- **Papel:** Aja como o comitê de priorização de portfólio da InovaTech, usando os pesos definidos no Prompt 3.
- **Restrições:** A decisão de cada um dos 8 projetos deve vir com 1 frase de "porquê"; não recomende cancelar um projeto só por estar com risco alto se o alinhamento estratégico e o ROI forem muito altos (ex.: Shield 2.0); não repita os dados brutos da tabela do case, só a conclusão.
- **Objetivo:** Aplicar os critérios de priorização (ROI, Alinhamento, Urgência, Risco) aos 8 projetos do portfólio e classificar cada um em CANCELAR, ACELERAR, PAUSAR/REVISAR ou MANTER, com justificativa curta.
- **Moldura:** Tabela: Projeto | Score (0-100) | Recomendação | Porquê (1 frase).
- **Panorama:** Os 8 projetos do case (Migração Cloud, Shield 2.0, Engenharia.AI, CRM Rebirth, LatAm Expansion, Auto-Update System, Legacy Harmonizer, Portal InovaNews), com seus dados de ROI, custo, consumido, disponível e risco qualitativo.
- **Tom e Testes:** Tom objetivo e numérico, adequado para uma reunião de board de 30 minutos; teste a recomendação também contra a pergunta "isso libera caixa hoje ou não?".

**Prompt final aplicado:**
> "Aja como o comitê de priorização de portfólio da InovaTech, usando os pesos de ROI/Alinhamento/Urgência/Risco definidos anteriormente (Papel). Cada projeto precisa de 1 frase de justificativa; não cancele um projeto de risco alto se ROI e alinhamento forem muito altos; não repita os dados brutos da tabela (Restrições). Classifique os 8 projetos em CANCELAR, ACELERAR, PAUSAR/REVISAR ou MANTER (Objetivo). Tabela: Projeto | Score | Recomendação | Porquê (Moldura). Use os dados dos 8 projetos do case: Migração Cloud, Shield 2.0, Engenharia.AI, CRM Rebirth, LatAm Expansion, Auto-Update System, Legacy Harmonizer e Portal InovaNews (Panorama). Tom objetivo, numérico, para uma reunião de board de 30 minutos, testando também se a decisão libera caixa hoje (Tom e Testes)."

---

### Observação sobre iteração e HITL

Cada prompt foi refinado em pelo menos uma rodada (ajustando o Panorama com os números exatos do case e a Moldura para formato tabular), seguindo a técnica de **iteração** do framework. Todas as saídas foram tratadas como rascunho de consultoria — **revisão humana (HITL)** é obrigatória antes de qualquer decisão de cancelamento/aceleração de projeto ser levada ao board, especialmente porque os scores de Urgência e Alinhamento Estratégico usados no protótipo (pasta `03-prototipo`) são estimativas qualitativas, não dados fechados de sistema.
