# Fleet Analytics — BI para gestão de equipamentos

**Estudo demonstrativo com dados 100% sintéticos.** Não contém indicadores, custos ou informações de empresas reais.

**Projeto técnico:** [Fleet Analytics](https://github.com/Peruzini/bi-analytics-portfolio/tree/main/projetos/fleet-dax-advanced) · [PBIP editável](https://github.com/Peruzini/bi-analytics-portfolio/tree/main/powerbi/fleet) · [Modelo dimensional](https://github.com/Peruzini/bi-analytics-portfolio/blob/main/projetos/fleet-dax-advanced/docs/modelo-dimensional.md)

## Problema que orienta o estudo

Em uma operação com múltiplos equipamentos, produção e metas não explicam sozinhas a performance. Para priorizar ações, é preciso relacionar **disponibilidade, horas operadas, falhas, manutenção, abastecimento, custos e criticidade** por equipamento e período, preservando o contexto dos filtros.

## Solução implementada no Git

- **Modelo dimensional** com `DimData` e `DimEquipamento` relacionadas a fatos de operação, manutenção, abastecimento e metas.
- **Power BI Project (PBIP)** com **4 páginas**: visão executiva, performance da frota, manutenção/Pareto e criticidade.
- **34 medidas DAX incorporadas ao modelo**, cobrindo produção, disponibilidade, utilização, produtividade, custo por tonelada, MTBF, MTTR, tendências e rankings.
- **Índice relativo de criticidade** com quatro componentes normalizados: disponibilidade (35%), custo por tonelada (25%), falhas (20%) e horas de perda/manutenção (20%).
- **Power Query e gerador Python** para a massa sintética; consultas SQL complementares e documentação de regras.

## O que o estudo permite investigar

| Pergunta de negócio | Análise implementada |
| --- | --- |
| Qual equipamento merece prioridade de análise? | Ranking e classe de criticidade |
| A produção atingiu o planejado? | Produção, metas e aderência |
| Onde o custo se concentra? | Combustível, manutenção e custo por tonelada |
| O desempenho está melhorando? | Comparações por período, acumulados e janelas móveis |

## Evidência e limites

| Evidência | Situação |
| --- | --- |
| [Arquivos PBIP / PBIR e modelo semântico](https://github.com/Peruzini/bi-analytics-portfolio/tree/main/powerbi/fleet) | Disponíveis e versionados |
| [Catálogo DAX e regras](https://github.com/Peruzini/bi-analytics-portfolio/tree/main/projetos/fleet-dax-advanced/dax) | Disponíveis, mas catálogo expandido não equivale às 34 medidas do PBIP |
| Abertura, refresh e interação no Power BI Desktop | **Ainda sem homologação final comprovada** |
| Capturas de tela reais de cada página | **Pendentes** |

O índice de criticidade é uma composição didática de critérios, não uma predição de falhas ou uma recomendação real de manutenção. O relatório foi estruturado para avaliação técnica; não existem resultados operacionais medidos em empresas.

**Competências evidenciadas:** Power BI, DAX, Power Query/M, modelagem dimensional, SQL, Python, métricas industriais e definição de regras de negócio.
