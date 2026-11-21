<div align="center">

# Rafael Peruzini

**Business Intelligence · Analytics Engineering · Planejamento e Dados**

Da necessidade operacional ao dado confiável: modelos, indicadores e soluções que possam ser testados, explicados e utilizados na tomada de decisão.

**Power BI / DAX** · **SQL / dbt / Snowflake** · **Python / PySpark** · **Automação**

[Projetos com evidências](#projetos-com-evidências) · [Experiência](#experiência) · [Projetos recentes](docs/PROJETOS_RECENTES_2026-11-21.md) · [Todos os repositórios](docs/REPOSITORY_CATALOG_2026-11-21.md)

</div>

Sou formado em **Engenharia de Minas** e **Ciência de Dados**, com experiência na **FGV IBRE**, em BI e soluções analíticas, e na **CSN**, em planejamento e indicadores operacionais. Trabalho na ligação entre regras de negócio, qualidade dos dados, automação e visualização, com foco em resultados que possam ser conferidos.

## Projetos com evidências

Três pontos de partida para avaliar meu trabalho. Cada estudo separa **o que está implementado**, **o que foi testado** e **o que ainda precisa de validação**.

| Projeto | O que foi desenvolvido | Evidência para conferir |
| --- | --- | --- |
| **[E-commerce Analytics — dbt + Power BI](https://github.com/Peruzini/analytics-engineering-snowflake-dbt)** | Pipeline com 6 fontes sintéticas, 7 marts, 39 medidas DAX e relatório de 4 páginas/50 visuais | [Estudo de caso](https://github.com/Peruzini/analytics-engineering-snowflake-dbt/blob/main/docs/PORTFOLIO_CASE_STUDY.md) · [Gates de validação](https://github.com/Peruzini/analytics-engineering-snowflake-dbt/blob/main/docs/MVP04D_RELEASE.md) |
| **[Fleet Analytics — BI operacional](case-studies/fleet-analytics.md)** | Modelo dimensional de equipamentos, custos, produção, manutenção e criticidade; PBIP com 34 medidas DAX | [Case e limitações](case-studies/fleet-analytics.md) · [PBIP editável](https://github.com/Peruzini/bi-analytics-portfolio/tree/main/powerbi/fleet) |
| **[EquipAnalytics — PySpark](case-studies/equipanalytics.md)** | Pipeline Bronze/Silver/Gold, regras de qualidade, reconciliação, SQL e Parquet | [Case e prévia](case-studies/equipanalytics.md) · [CI concluída](https://github.com/Peruzini/bi-analytics-portfolio/actions/runs/34867957046) |

**Evidência visual disponível — EquipAnalytics**

<a href="https://github.com/Peruzini/bi-analytics-portfolio/tree/main/projetos/big-data-equipamentos"><img src="https://raw.githubusercontent.com/Peruzini/bi-analytics-portfolio/main/projetos/big-data-equipamentos/assets/preview.svg" alt="EquipAnalytics: indicadores de uma amostra sintética controlada e reconciliação entre registros válidos, rejeitados e duplicados" width="680"></a>

*Prévia estática de 10 registros sintéticos com valores esperados; não é captura de Power BI nem resultado visual de uma execução Spark. [Dados e validação](https://github.com/Peruzini/bi-analytics-portfolio/blob/main/projetos/big-data-equipamentos/docs/validacao.md).*

### Como ler as evidências

- **Código e modelo no Git** comprovam implementação, não funcionamento em ambiente final.
- **CI PASS** comprova testes daquele commit e daquele ambiente; não equivale à aprovação de um dashboard por usuários.
- **Capturas reais do Power BI Desktop** ainda são pendentes para os relatórios Fleet e E-commerce. Não substituo essas capturas por imagens ilustrativas.

Para mais casos, veja [CYBER ÁTRIA](case-studies/cyber-atria.md), [VTT Scene Compiler](case-studies/vtt-scene-compiler.md) e [GanttFlow](case-studies/ganttflow.md). Nos projetos privados, apenas o escopo publicável aparece aqui.

## Projetos mais recentes — novembro de 2026

Além dos cases de BI, estou desenvolvendo produtos de software e ferramentas com fluxos de teste, documentação e evolução incremental. O **estado de cada projeto é explicitado**, sem confundir protótipo, PR de desenvolvimento e entrega em produção.

| Projeto | Escopo demonstrável | Situação |
| --- | --- | --- |
| **[Competir — eventos e fotografias](docs/PROJETOS_RECENTES_2026-11-21.md#competir--eventos-e-fotografias)** | Plataforma para organizadores e fotógrafos: galerias, inscrições simuladas, painéis operacionais e backup/restauração sintéticos | Protótipo local; OPS-02E2 integrada à `main`; pagamentos reais em HOLD |
| **[Noite Infinita — jogo HTML5](docs/PROJETOS_RECENTES_2026-11-21.md#noite-infinita--jogo-html5)** | Jogo de sobrevivência para desktop/mobile, arte, progressão, armas e inimigos | Release candidate privado na `main`; melhorias GD-07/08 em PRs draft |
| **[Forja WP Bridge](docs/PROJETOS_RECENTES_2026-11-21.md#forja-wp-bridge--integração-chatgpt-e-wordpress)** | Pesquisa de integração ChatGPT/WordPress, OAuth, multiusuário e segurança em staging | Provas e branches em desenvolvimento; conexão real ainda não homologada |
| **[Warhammer TTS Narrator](docs/PROJETOS_RECENTES_2026-11-21.md#warhammer-tts-narrator--pesquisa-em-voz-ia)** | Pesquisa de narração PT-BR com TTS open-source, Colab e Drive | Pesquisa em PRs draft; não há versão de produção homologada |

[Ver panorama atualizado, limites e evidências](docs/PROJETOS_RECENTES_2026-11-21.md).

## Todos os repositórios

[**Catálogo dos 29 repositórios da conta — conferência em 21/11/2026**](docs/REPOSITORY_CATALOG_2026-11-21.md) — projetos ativos, cases, trabalhos acadêmicos e forks de terceiros. Os repositórios privados só são acessíveis a quem tem permissão. O inventário anterior de 19/10 permanece como registro histórico.

## Produtos digitais e portfólio web

### Forja Mineira D20 — WordPress e evolução de produto

[Ver código e documentação](https://github.com/Peruzini/forja-mineira-d20) · [Site público](https://forjamineirad20.com.br/)

Projeto editorial e técnico com desenvolvimento e manutenção de plugins PHP/CSS/JavaScript, organização de conteúdo, SEO e estratégias de atualização e rollback. A integração própria Forja WP Bridge permanece em pesquisa; **a conexão MCP real no Chat normal não está homologada**.

### Portfólio Web — desenvolvimento para negócios

[Ver repositório](https://github.com/Peruzini/portfolio-web)

Sites institucionais e landing pages em PHP, HTML, CSS e JavaScript, com atenção a responsividade, formulários e implantação. Os [materiais de apresentação](https://github.com/Peruzini/portfolio-web/tree/main/docs/previews) são prévias de projeto, não validação de funcionamento dos sites.

## R&D e produtos em desenvolvimento

Além dos estudos de portfólio, desenvolvo projetos de pesquisa, ferramentas e automações que complementam meu trabalho em dados, arquitetura de software e IA aplicada.

| Projeto | Foco | Evidência pública |
| --- | --- | --- |
| **GanttFlow for Power BI** | Produto de Gantt para planejamento, baseline e análise de desvios no Power BI | [Case study](case-studies/ganttflow.md) |
| **VTT Scene Compiler** | Pipeline assistido por IA para reconstrução estrutural de battlemaps | [Case study com arquitetura e benchmarks](case-studies/vtt-scene-compiler.md) |
| **CYBER ÁTRIA** | Scanner passivo e autorizado com saída estruturada para revisão | [Case study com pipeline e validação prática](case-studies/cyber-atria.md) |
| **API de gerenciamento do Facebook** | Integração entre Página do Facebook, Meta Graph API e clientes autorizados | [Repositório público](https://github.com/Peruzini/API-de-gerenciamento-do-Facebook) |

> A visibilidade dos repositórios varia de acordo com o projeto. Quando houver dados internos ou evidências não publicáveis, compartilho apenas material autorizado.

## Outros estudos de dados

| Projeto | Objetivo | Evidências |
| --- | --- | --- |
| [Indicadores de projetos](https://github.com/Peruzini/bi-analytics-portfolio/tree/main/projetos/indicadores-projetos) | Acompanhar backlog, prazos e entregas | PBIP, DAX e referências numéricas |
| [Marketing Analytics](https://github.com/Peruzini/bi-analytics-portfolio/tree/main/projetos/marketing-analytics) | Avaliar aquisição, conversão, CAC e ROAS | SQL, Python, dados sintéticos e medidas DAX |
| [Análise comercial](https://github.com/Peruzini/bi-analytics-portfolio/tree/main/projetos/analise-comercial) | Analisar receita e margem por loja, categoria e período | PBIP, SQL, transformação e conciliação |
| [NBA Data Analytics](https://github.com/Peruzini/M3-NBA-DataAnalytics-SQL) | Análise exploratória e consultas relacionais | SQL e projeto acadêmico em equipe |

## Stack

| Área | Tecnologias e práticas |
| --- | --- |
| **Business Intelligence** | Power BI, DAX, Power Query/M, modelagem dimensional, dashboards, KPIs |
| **Analytics Engineering** | SQL, dbt, Snowflake, Oracle, SQL Server, transformação, testes e regras de negócio |
| **Data Engineering** | Python, pandas, PySpark, Spark SQL, Parquet, AWS Athena, Databricks |
| **Automação e integração** | APIs, requests, Power Automate, SharePoint, rotinas Python |
| **IA aplicada a Analytics** | Snowflake Cortex, validação de respostas, preparação de contexto e casos de uso analíticos |
| **Engenharia de software** | Git, GitHub, branches, pull requests, GitHub Actions, testes e documentação |
| **Web / produto** | PHP, HTML, CSS, JavaScript, WordPress, Node.js |
| **Negócio** | Levantamento de requisitos, planejamento, indicadores, análise de desvios e melhoria de processos |

## Como trabalho com dados

1. Entendo a decisão de negócio e transformo a necessidade em métricas e regras verificáveis.
2. Investigo a origem dos dados e valido chaves, duplicidades, nulos, agregações e consistência entre fontes.
3. Estruturo as transformações e o modelo antes de levar a informação para a camada de visualização.
4. Comparo os resultados com referências e critérios de aceite antes da entrega.
5. Versiono código, documentação e mudanças relevantes para manter rastreabilidade.

## Experiência

**FGV IBRE — Analista de BI**  
Power BI, SQL/Oracle, Snowflake, automações, indicadores, qualidade de dados e apoio a áreas de negócio.

**CSN — Técnico Especialista em Planejamento**  
Planejamento, KPIs operacionais, análise de equipamentos, acompanhamento de desempenho e suporte à tomada de decisão.

---

Os projetos demonstrativos utilizam dados próprios, públicos ou sintéticos e não expõem informações confidenciais de empregadores ou clientes.
