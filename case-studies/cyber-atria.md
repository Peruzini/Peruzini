# CYBER ÁTRIA — Case Study de Automação e Qualidade de Dados

## Contexto

CYBER ÁTRIA é um scanner passivo desenvolvido para apoiar a análise técnica inicial de sites previamente autorizados.

O objetivo não é explorar vulnerabilidades. O sistema coleta sinais limitados e estruturados, registra evidências e gera dados que podem ser revisados antes de qualquer uso comercial.

## Escopo técnico

O scanner trabalha com sinais como:

- resposta HTTP;
- cabeçalhos de segurança;
- handshake TLS e certificado;
- consultas DNS de e-mail somente quando explicitamente autorizadas;
- consolidação em CSV/JSON;
- classificação determinística de achados;
- fila de revisão humana.

O projeto evita crawling, login, exploração, descoberta de ativos ou ações ofensivas.

## Pipeline

O fluxo evoluiu para suportar:

1. intake offline de leads autorizados;
2. validação de domínio e opt-out;
3. lote manual de até 100 domínios;
4. coleta sequencial controlada;
5. persistência local dos relatórios;
6. geração de fila de revisão comercial;
7. rastreabilidade via hashes e GitHub Actions.

## Validação prática

Em um piloto real documentado com seis domínios autorizados:

- **6/6 análises foram concluídas**;
- **0 erros** de execução;
- **8 sinais técnicos indicativos** foram registrados;
- os seis resultados foram vinculados aos respectivos leads;
- nenhuma abordagem comercial foi liberada automaticamente.

O piloto também revelou uma limitação importante: a classificação técnica, isoladamente, não era suficiente para priorização comercial. Essa evidência passou a orientar a próxima etapa do produto.

## Qualidade e testes

A evolução do projeto foi acompanhada por uma suíte automatizada crescente. No marco do piloto, a CI registrou mais de mil testes aprovados, com separação entre validações offline e execuções reais autorizadas.

## O que este projeto demonstra

- Python;
- HTTP, TLS e DNS;
- CSV/JSON e contratos de dados;
- validação e classificação determinística;
- testes automatizados;
- GitHub Actions;
- desenho de workflows;
- rastreabilidade;
- transformação de sinais técnicos em dados consumíveis por processos de negócio.

## Princípios

O projeto foi construído com três restrições centrais:

- coleta somente em domínio autorizado;
- achado técnico não é tratado como vulnerabilidade confirmada;
- revisão humana permanece obrigatória antes de qualquer ação comercial.

> O repositório de desenvolvimento é privado. Este case publica somente arquitetura, métricas agregadas e decisões que podem ser compartilhadas sem expor alvos, dados internos ou detalhes operacionais sensíveis.
