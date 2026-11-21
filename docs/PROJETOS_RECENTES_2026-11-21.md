# Projetos recentes — panorama de novembro de 2026

**Corte:** 21/11/2026. Resumo público de escopo e maturidade, baseado em repositórios, commits e PRs acessíveis ao titular. Os repositórios privados não têm o código exposto por este documento.

## Competir — eventos e fotografias

**Repositório:** `Peruzini/marketplace-fotografias` (privado).

Plataforma em desenvolvimento para organizadores de eventos e fotógrafos: cadastro e minissites de eventos, inscrições de teste, categorias/lotes, convites de cobertura, galerias com prévias e marca d'água, painéis de gestão, notificações e controles de recuperação.

**Situação em 21/11:** protótipo técnico local, sem produção comercial. Os blocos UX-OPS-02E/PERF-OPS-01D foram integrados; o pacote sintético OPS-02E2 também aparece integrado à `main` no PR #50. OPS-02F é um PR draft para prova offline de backup em Windows; não está integrado. **Pix/split real, cobrança e reconhecimento facial real estão em HOLD.** Testes sintéticos ou recuperação local não provam backup offsite operacional.

## Noite Infinita — jogo HTML5

**Repositório:** `Peruzini/noite-infinita-youtube` (privado).

Jogo de sobrevivência em HTML5/JavaScript para navegador, com personagem próprio, armas, passivas, inimigos, HUD, melhorias visuais e uso em desktop/celular.

**Situação em 21/11:** o release candidate privado GD-06C foi incorporado à `main` pelo PR #57. Abertura cinematográfica, transição premium, hordas crescentes, modo Noite Eterna, estatísticas e top 10 global são incrementos em PRs empilhados **draft** (GD-07C/08A/08B/08C/08D), não versões homologadas na `main`. Um protótipo para navegador não equivale à certificação YouTube Playables.

## Forja WP Bridge — integração ChatGPT e WordPress

**Repositório:** `Peruzini/forja-mineira-d20` (público).

Frente de P&D dentro do produto Forja Mineira D20 para integrar tarefas WordPress ao ChatGPT por uma aplicação MCP, com testes de autenticação, OAuth, isolamento de usuários e infraestrutura de staging.

**Situação em 21/11:** investigação e contrato de integração documentados. A conexão direta de ferramentas MCP ao Chat normal **não foi homologada** (diagnóstico FWB-05). A linha FWB-REG-01 até FWB-REG-04D-R1 está em PRs empilhados **draft**; Keycloak, PostgreSQL, CIMD e gateway seguem condicionados à validação de infraestrutura e integração real. Não interpretar experimentos de laboratório como publicação oficial do plugin.

## Warhammer TTS Narrator — pesquisa em voz IA

**Repositório:** `Peruzini/warhammer-tts-narrator` (privado).

Pesquisa de geração de narrações em português brasileiro com ferramentas TTS open-source e experimentos planejados em Colab/Drive para vídeos temáticos.

**Situação em 21/11:** a `main` contém o commit inicial; o bootstrap e os experimentos TTS-02, TTS-03 (Colab/Chatterbox) e TTS-04 (Qwen3-TTS) estão em PRs **draft**. Não há resultado de narração aprovado para distribuição nem pipeline de produção comprovado.

## Outras frentes técnicas ativas

- **Radar Swing Trade B3:** radar de pesquisa e monitoramento; EDGE-01A/01B em branches/PRs de pesquisa para coberturas históricas e replay sem viés de antecipação. Nenhuma negociação executada automaticamente pelo software.
- **VTT Scene Compiler:** reconstrução estrutural de mapas com ferramentas de visão e validações; preservar estado de branches e aceites específicos.
- **Música IA Studio:** infraestrutura de edição audiovisual e catálogo de conteúdo; homologação de componentes não equivale a uma solução end-to-end integralmente validada.
- **Analytics Engineering:** e-commerce sintético com dbt/DuckDB e PBIP, MVP-04D; validação local foi informada, porém prova de abertura/round-trip do Power BI Desktop continua pendente.

## Convenções de entrega

`IMPLEMENTADO` = código presente na branch. `CI PASS` = testes automáticos daquele commit. `MERGED` = integrado ao ramo de destino. `HOMOLOGADO` = aceite explícito no escopo declarado. `HOLD` = não operacional/sem autorização para avançar. **Nenhum desses marcos implica outro automaticamente.**

Este panorama não contém imagens, mídias ou dados privados, credenciais, métricas comerciais não medidas nem informações de terceiros. Para auditorias detalhadas, utilizar as evidências no repositório respectivo com acesso autorizado.
