# VTT Scene Compiler — Case Study de Visão Computacional

## Contexto

VTT Scene Compiler é um projeto privado de P&D que investiga como reduzir o trabalho manual necessário para transformar um battlemap em uma cena estrutural utilizável em Virtual Tabletop (VTT).

A hipótese central é que visão computacional e reconstrução geométrica podem identificar paredes e portais e gerar uma representação estrutural que precise apenas de revisão humana.

## Arquitetura

A linha de processamento estudada é:

```text
Battlemap
  -> preprocessing / grid scale
  -> semantic vision
  -> wall / portal predictions
  -> structural reconstruction
  -> geometry optimizer
  -> topology validation
  -> SceneGraph
  -> VTT compiler
```

O SceneGraph foi desenhado para ser independente de um VTT específico.

## Metodologia

O trabalho foi dividido em POCs progressivas:

- baseline com visão computacional clássica;
- prior semântico genérico;
- treinamento orientado a estruturas próprias de VTT;
- hard negatives e holdout independente;
- reconstrução estrutural e topologia.

O projeto usa benchmarks e critérios objetivos para evitar avançar para produto antes de existir evidência técnica suficiente.

## Evidência atual

Em holdout independente registrado no projeto, a etapa semântica atingiu aproximadamente:

- **60,69%** de precisão mediana de paredes;
- **71,07%** de recall mediano;
- **66,85%** de F1 mediano;
- razão mediana de segmentos de **4,12x** em relação à referência estruturada.

Cinco de sete mapas positivos ficaram entre aproximadamente **63% e 92% de F1 de paredes**.

Esses resultados representam progresso técnico, mas permanecem abaixo do gate definido para produto.

## Critérios de produto

Antes de uma integração final com VTT, o projeto estabeleceu metas como:

- precisão de paredes >= 93%;
- recall de paredes >= 95%;
- razão de segmentos <= 1,5x;
- recall de portais >= 90%;
- tempo mediano até uma cena jogável inferior a 3 minutos;
- redução de trabalho manual de pelo menos 80%.

## O que este projeto demonstra

- Python aplicado a visão computacional e ML;
- desenho experimental por POCs;
- definição de métricas e gates;
- validação em holdout;
- arquitetura de pipeline;
- governança de datasets e fontes;
- GitHub Actions e documentação de pesquisa.

## Limites

O projeto não é apresentado como produto final. A exportação para Foundry/VTT permanece deliberadamente posterior à validação estrutural.

> O código, datasets e materiais de avaliação permanecem privados. Este documento publica apenas arquitetura, metodologia e resultados agregados que podem ser compartilhados.
