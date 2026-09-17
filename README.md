# EvoluaSeguro — Sistema de Medição e Análise de Software (SMAS)

Projeto Prático Integrador · Plano e Painel de Medição de Software

**Painel de variáveis de controle:** https://digo1214.github.io/evoluaseguro-smas/

---

## Sobre o projeto

O **EvoluaSeguro** é uma plataforma de seguros (cotação, emissão de apólice, cobrança de prêmio,
renovação e sinistros) adotada como objeto de estudo para construir, do zero, um plano completo
de medição e análise de qualidade de software.

O diagnóstico inicial: o sistema custou **R$ 180.000** para ser construído e, no primeiro ano de
operação, a falta de qualidade custou **R$ 150.800** — 83,8% do valor de construção. A investigação
mostrou que a causa não era capacidade técnica da equipe, mas a **ausência de um sistema de medição**:
4 de cada 10 defeitos chegavam ao cliente, e 63% dos defeitos críticos escapavam de todos os filtros
de verificação.

## O painel

O painel publicado reúne, em uma única camada de leitura, as variáveis de controle do Ciclo 2:

| Grupo | Indicadores |
|---|---|
| **Fluxo** | Lead Time, Cycle Time (média e percentil 85), Throughput, WIP |
| **Valor agregado (EVMS)** | PV, EV, AC, SPI, CPI, EAC, VAC |
| **Escopo** | Burn-down real × ideal |
| **Qualidade** | Cobertura de testes, DRE, defeitos críticos em produção |

Cada gráfico traz um rodapé **"Decisão que apoia"**, que registra a ação gerencial associada —
aplicação do princípio de que métrica sem decisão associada é relatório, e não controle.

O painel é interativo: passe o cursor sobre os gráficos para inspecionar valores por sprint e use
**"Ver dados em tabela"** para consultar a série numérica completa.

## As sete etapas

| Etapa | Entrega | Resultado central |
|---|---|---|
| 1 | Contextualização e viabilidade econômica | CNQ de R$ 150.800 (83,8% do investimento) |
| 2 | Classificação e densidade de defeitos | 1,55 def/KLOC · 63,2% dos críticos escapam |
| 3 | Atributos de qualidade (ISO/IEC 25010) | 5 atributos priorizados · 10 requisitos rastreados |
| 4 | Plano de testes e métricas de cobertura | DRE 61,3% · causa raiz na Definição de Pronto |
| 5 | Dashboard de variáveis de controle | SPI e CPI 0,91 · EAC R$ 105.380 |
| 6 | Comunicação, time e código de ética | Métricas do sistema, nunca da pessoa |
| 7 | Framework e plano consolidado | MPS.BR + ISO/IEC 25010 · 28 indicadores |

## Resultado projetado

| | Ano 1 | Ano 2 | Ano 3 |
|---|---|---|---|
| Custo da Não-Qualidade | R$ 150.800 | R$ 56.933 | R$ 11.800 |
| % do investimento | 83,8% | 31,6% | 6,6% |

Retorno de aproximadamente **2,7×** sobre o investimento em qualidade já no segundo ano.

## Modelos de referência

- **MPS.BR (MPS-SW)** — modelo de processo. O processo *Medição (MED)* está no nível F, e a
  avaliação de aderência indica 5 dos 7 resultados esperados já atendidos.
- **ISO/IEC 25010** — modelo de qualidade de produto (5 atributos priorizados).
- **GQM (Goal–Question–Metric)** — método de ligação entre objetivo de negócio e métrica coletada.

## Nota sobre os dados

O EvoluaSeguro é um **estudo de caso**, e os dados são hipotéticos. Eles são, porém, internamente
consistentes: os 12 defeitos críticos que escaparam correspondem às 12 falhas da Etapa 1;
12 × R$ 3.333 reproduz exatamente os R$ 40.000 de manutenção corretiva do Ano 1; e a série de
fluxo satisfaz a Lei de Little em todos os sprints.

## Equipe

- Rodrigo Bispo do Nascimento
- Fernando Alonso Mota Pinho
- Ronald de Jesus Campos
- Daniel Barros Moreira
- Edvaldo Cipriano Bittencourt Junior

Docente: Nadja Soraya Torres Dias
