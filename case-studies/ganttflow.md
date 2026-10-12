# GanttFlow for Power BI — Case Study

## Contexto

GanttFlow é um produto em desenvolvimento para visualização e análise de cronogramas dentro do Power BI.

A proposta nasceu de uma necessidade recorrente em planejamento e controle de projetos: visualizar tarefas, marcos, progresso e desvios sem depender de uma ferramenta separada para cada análise executiva.

## Problema

Visuais de Gantt básicos costumam mostrar apenas uma linha do tempo. Para planejamento e controle, isso é insuficiente quando o usuário precisa responder perguntas como:

- quais tarefas estão atrasadas;
- como o cronograma atual se compara à baseline;
- onde existem desvios relevantes;
- quais pacotes de trabalho concentram risco;
- como o cronograma reage aos filtros do relatório Power BI.

## Direção do produto

O desenho do GanttFlow prevê:

- hierarquia de tarefas e work packages;
- datas de início e fim;
- progresso;
- milestones;
- status e responsáveis;
- baseline versus cronograma atual;
- indicadores de variação;
- filtros e cross-highlighting nativos do Power BI;
- grade de tarefas e timeline configuráveis.

## Modelagem

O contrato de dados foi pensado para aceitar campos como:

- Task / Task ID;
- Parent ID;
- Start / End;
- Progress;
- Project;
- Status;
- Owner;
- Category;
- Milestone.

A intenção é manter uma camada de dados flexível para fontes como Excel, SQL, SharePoint, SAP, Jira, Primavera e Microsoft Project, desde que os dados sejam transformados para o contrato esperado pelo visual.

## Decisões técnicas

Os princípios atuais são:

1. comportamento alinhado ao ecossistema Power BI;
2. leitura executiva sem excesso de complexidade visual;
3. foco em diagnóstico rápido de cronograma;
4. modelo de dados flexível;
5. arquitetura consciente dos requisitos de distribuição e certificação de visuais Power BI.

## Status

O projeto está em fase de definição de MVP e arquitetura. A especificação de produto, contrato de dados e roadmap já foram estruturados; a implementação do visual ainda não é apresentada como produto concluído.

## Competências demonstradas

- Power BI e modelagem analítica;
- entendimento de planejamento e controle;
- definição de produto orientado a problema;
- desenho de contrato de dados;
- documentação técnica;
- versionamento com Git/GitHub.

> O repositório de desenvolvimento é privado. Este case apresenta apenas o escopo técnico e as decisões de produto que podem ser compartilhadas publicamente.
