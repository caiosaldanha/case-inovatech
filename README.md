# Case Final — Consultoria de PMO para a InovaTech

Esta pasta contém os entregáveis do **Case Final** do caderno "Inteligência Artificial para Líderes" (`CADERNO-ATIVIDADES-02.html`), aplicando como "empresa" o **Estudo de Caso: O Colapso Silencioso da InovaTech** (`Estudo de Caso_ O Colapso Silencioso da InovaTech.md`).

Do desafio de consultoria de PMO do estudo de caso, foram executados os itens **1 a 4** (Diagnóstico do PMO, Quick Wins, Critérios de Priorização e Saneamento de Portfólio). O **item 5** (Relatório de Impacto/ROI do PMO em 12 meses) foi **deliberadamente não executado**, por decisão de escopo.

## Estrutura (um entregável do Case Final por pasta)

| Pasta | Entregável do Case Final | Conteúdo |
|---|---|---|
| `01-problema/` | "1 página descrevendo o problema escolhido e por que é relevante" | `problema.md` |
| `02-prompts/` | "Os prompts utilizados, estruturados com o framework P.R.O.M.P.T" | `prompts.md` — 4 prompts (um por item do desafio: diagnóstico, quick wins, critérios, saneamento) |
| `03-prototipo/` | "O protótipo funcional gerado (arquivo HTML...)" | `dashboard-pmo.html` — dashboard interativo standalone (abra direto no navegador); `data/portfolio.json` — dados dos 8 projetos, reutilizáveis em planilha/automação |
| `04-reflexao-final/` | "Reflexão final de até 10 linhas sobre riscos, limitações e próximos passos" | `reflexao.md` |

## Como usar o protótipo

Abra `03-prototipo/dashboard-pmo.html` diretamente no navegador (duplo clique — não depende de servidor). Ele traz:

- O diagnóstico do modelo de PMO recomendado (Diretivo, evoluindo para Controlador);
- Os 3 quick wins de 30 dias;
- Os indicadores de sangramento financeiro do case;
- Uma matriz de priorização **interativa**: sliders de peso para ROI, Alinhamento Estratégico, Urgência e Risco recalculam, em tempo real, o score e a recomendação (ACELERAR / MANTER / PAUSAR-REVISAR / CANCELAR) de cada um dos 8 projetos, além do caixa liberado ao cancelar os projetos recomendados.

## Resumo da recomendação (com os pesos padrão: ROI 30% · Alinhamento 35% · Urgência 20% · Risco 15%)

- **Cancelar:** Legacy Harmonizer, Portal "InovaNews" → libera R$ 700 mil de orçamento disponível.
- **Acelerar:** Migração Cloud (SaaS), Shield 2.0 (Security), Engenharia.AI.
- **Pausar/Revisar:** LatAm Expansion, CRM Rebirth.
- **Manter/Concluir:** Auto-Update System.

O racional completo de cada decisão está no dashboard (`03-prototipo/dashboard-pmo.html`, seção 4) e nos prompts (`02-prompts/prompts.md`).
