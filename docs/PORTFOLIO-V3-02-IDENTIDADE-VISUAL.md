# PORTFOLIO-V3-02 — Identidade visual (proposta para revisão)

## Direção
BI e dados como eixo principal; desenvolvimento e automação como competências complementares. A proposta não presume resultados de contratação. Referências: [Ruban Kumar](https://github.com/rubankumar296-maker/portfolio), [Matt Hummel](https://github.com/matthummel-pa/matthummel-theme) e [Data With Baraa](https://github.com/DataWithBaraa/sql-data-warehouse-project).

## Prévia
![Banner profissional: Rafael Peruzini, dados, BI e soluções de software](../assets/brand/banner-v3.svg)

Em telas estreitas, preservar também o nome e as áreas como texto HTML/Markdown acessível no README (V3-03). Não depender apenas do texto incorporado ao SVG.

## Tokens
| Token | Valor | Uso |
| --- | --- | --- |
| Navy | #0B192B | Fundo |
| Petroleum | #103C49 | Fundo secundário |
| Cyan | #67D8EA | Acento e destaque |
| White | #FFFFFF | Texto principal |
| Mist | #E3EEF3 | Texto secundário |
| Muted | #B8D6DF | Metadados |
| Typeface | Arial, Helvetica, sans-serif | Sem fontes externas |
| Grid | 8px | Espaçamento base |
| Radius | 24px | Capas |

## Cards
Proporção 16:9 (1200 × 675), título conciso, competência principal e status textual no Markdown. Uma identidade por família, sem depender da cor para comunicar status. Priorizar capturas reais em moldura consistente. Diagramas e capas conceituais devem ser identificados como tais. Não inserir números, badges de testes ou alegações sem evidência. Manter alt text e link de texto para cada case.

Destaques propostos: Fleet Analytics, E-commerce Analytics, Forja Mineira D20 e Cyber Átria. Cases complementares: EquipAnalytics, Competir, Noite Infinita, Forja WP Bridge. Não publicar dados privados nem promover pesquisa a produção.

## Validação e gates
SVG autocontido, viewBox fixo com escala proporcional, fundo opaco, sem dependência remota, scripts ou fontes web. Contrastes calculados pelo método WCAG; ver registro abaixo. O banner não substitui navegação textual. Revisão visual humana no GitHub desktop/mobile, temas claro/escuro, ainda pendente. README principal intacto até V3-03. Sem merge automático.

## Pendências transferidas
V3-04: capas definitivas; V3-05: capturas reais; V3-07: evidências; V3-10: responsividade e acessibilidade; V3-11: benchmark pós-implementação.

### Contraste teórico (texto/fundo)

| Texto | Navy | Petroleum |
| --- | ---: | ---: |
| #FFFFFF | 17.67:1 | 11.90:1 |
| #E3EEF3 | 14.97:1 | 10.08:1 |
| #B8D6DF | 11.55:1 | 7.78:1 |
| #67D8EA | 10.59:1 | 7.13:1 |

Cálculo de luminância relativa sRGB, não teste de renderização. Todos os pares de texto excedem 4,5:1.
