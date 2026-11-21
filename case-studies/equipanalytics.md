# EquipAnalytics — Engenharia de dados para análise operacional

**Estudo demonstrativo com dados 100% sintéticos.** O domínio é consumo estimado de equipamentos, sem dados reais de empresas ou clientes.

[Projeto e código](https://github.com/Peruzini/bi-analytics-portfolio/tree/main/projetos/big-data-equipamentos) · [Testes e documentação](https://github.com/Peruzini/bi-analytics-portfolio/blob/main/projetos/big-data-equipamentos/docs/validacao.md) · [Registro persistente de execução](https://github.com/Peruzini/bi-analytics-portfolio/blob/main/projetos/big-data-equipamentos/results/ci-100k.json)

## O desafio

Como disponibilizar indicadores confiáveis quando os dados de origem têm **duplicações, timestamps inválidos, volumes inconsistentes e identificadores desconhecidos**? Sem controle de qualidade, o dashboard pode apresentar uma leitura precisa de informações incorretas.

## Solução

Pipeline em **PySpark e Spark SQL**, com persistência em **Parquet**:

`Geração/CSV → Bronze → validação e deduplicação → Silver + quarentena → Gold → CSV agregado para BI`

A implementação inclui geração determinística, regras de validação, reconciliação de contagens, ranking de equipamentos e indicadores por unidade e categoria. O consumo horário é calculado como **litros totais ÷ horas totais**, evitando médias simples de razões.

## Evidência visual — amostra controlada

![EquipAnalytics: indicadores de dez registros fictícios](https://raw.githubusercontent.com/Peruzini/bi-analytics-portfolio/main/projetos/big-data-equipamentos/assets/preview.svg)

*Visualização estática dos resultados esperados de 10 registros de teste, não uma captura do Power BI nem do processamento de 100 mil eventos.*

## Evidência de execução reproduzível

Em [14/09/2026, a execução GitHub Actions #34867957046](https://github.com/Peruzini/bi-analytics-portfolio/actions/runs/34867957046) foi concluída com sucesso no commit `7c6576f3`:

| Medida | Valor observado |
| --- | ---: |
| Testes aprovados | **7** |
| Eventos únicos gerados | **100.000** |
| Registros Bronze, com versões | 100.200 |
| Registros válidos Silver | 99.698 |
| Rejeições | 302 |
| Versões duplicadas | 200 |

**Reconciliação:** 100.200 = 99.698 válidos + 302 rejeitados + 200 versões duplicadas. O registro JSON preserva SHA, duração parcial, versão do Spark e contagens.

## Limites declarados

A execução ocorreu em **Spark local, em uma única máquina de CI**. Não demonstra cluster distribuído, benchmark de 1/10 milhões, análise com dados corporativos ou dashboard homologado no Power BI Desktop. Alertas são sinais para investigação e não diagnóstico de fraude ou falha mecânica. Nenhum ganho financeiro foi estimado.

**Competências evidenciadas:** PySpark, Spark SQL, Parquet, validação e reconciliação de dados, testes, GitHub Actions e modelagem de indicadores para BI.
