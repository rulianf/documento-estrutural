# Documentação da Empresa — Engenharia de Software com IA

Repositório com o método de trabalho dos três sócios: o que produzir em cada fase, com qual template e com qual critério de passagem. Ele adapta a engenharia clássica (entendimento do negócio, requisitos, projeto, construção, testes, implantação) a uma empresa pequena que usa IA no dia a dia.

> **Status:** rascunho v0.1. O que é decisão dos sócios e o que ainda é proposta está em [04-gestao/status-do-documento.md](04-gestao/status-do-documento.md).

## Por onde começar

1. Leia [os princípios e os níveis de formalização](00-fundamentos/01-principios-e-niveis.md).
2. Veja [o ciclo de vida e os portões](00-fundamentos/02-ciclo-de-vida-e-portoes.md).
3. Em cada trabalho, siga a página da fase em `01-fases/` e copie os templates de `02-templates/`.

## Estrutura

```text
documentacao-empresa/
├── README.md
├── 00-fundamentos/            Princípios, ciclo de vida e catálogo de documentos
├── 01-fases/                  Uma página por fase: objetivo, dono, atividades, portão
├── 02-templates/              Templates para copiar, organizados por fase
│   ├── fase-1-levantamento/
│   ├── fase-2-especificacao/
│   ├── fase-3-desenho-tecnico/
│   ├── fase-5-validacao/
│   └── fase-6-operacao/
├── 03-convencoes/             IDs, versões, pastas por cliente e contexto para a IA
│   └── contexto-para-ia/
├── 04-gestao/                 Uso de IA por fase, indicadores, pendências e status
└── 05-pilotos/                Exemplos preenchidos (escritório de advocacia)
```

A fase 4 (construção) não tem template próprio: o resultado é código no repositório, guiado pelo [plano de tarefas](02-templates/fase-3-desenho-tecnico/plano-de-tarefas.md).

## Fases e donos

| # | Fase | Dono | Página | Templates |
| --- | --- | --- | --- | --- |
| 1 | Entendimento do negócio | Lucas | [fase 1](01-fases/fase-1-entendimento-do-negocio.md) | [levantamento](02-templates/fase-1-levantamento/levantamento-da-necessidade.md) |
| 2 | Especificação da solução | Rulian | [fase 2](01-fases/fase-2-especificacao-da-solucao.md) | [especificação](02-templates/fase-2-especificacao/especificacao-da-solucao.md) |
| 3 | Desenho técnico e plano de tarefas | Rulian | [fase 3](01-fases/fase-3-desenho-tecnico-e-tarefas.md) | [desenho](02-templates/fase-3-desenho-tecnico/desenho-tecnico.md), [dados](02-templates/fase-3-desenho-tecnico/modelo-de-dados.md), [ADR](02-templates/fase-3-desenho-tecnico/adr.md), [tarefas](02-templates/fase-3-desenho-tecnico/plano-de-tarefas.md), [testes](02-templates/fase-3-desenho-tecnico/plano-de-testes.md) |
| 4 | Construção | Breno | [fase 4](01-fases/fase-4-construcao.md) | — |
| 5 | Validação e aceite | Breno, com Lucas e Rulian | [fase 5](01-fases/fase-5-validacao-e-aceite.md) | [relatório](02-templates/fase-5-validacao/relatorio-de-testes.md), [aceite](02-templates/fase-5-validacao/registro-de-entrega-e-aceite.md) |
| 6 | Implantação e operação | Breno | [fase 6](01-fases/fase-6-implantacao-e-operacao.md) | [implantação](02-templates/fase-6-operacao/plano-de-implantacao-e-reversao.md), [runbook](02-templates/fase-6-operacao/runbook.md), [demandas](02-templates/fase-6-operacao/registro-de-demanda-e-incidente.md) |

## Convenções e gestão

- [Identificadores e rastreabilidade](03-convencoes/identificadores-e-rastreabilidade.md)
- [Versões e status dos documentos](03-convencoes/versoes-e-status.md)
- [Pastas por cliente](03-convencoes/pastas-por-cliente.md)
- [Contexto da empresa para a IA](03-convencoes/contexto-para-ia/contexto-da-empresa.md)
- [Contexto do cliente e glossário](03-convencoes/contexto-para-ia/contexto-do-cliente.md)
- [Uso de IA por fase](04-gestao/uso-de-ia-por-fase.md)
- [Indicadores e melhoria contínua](04-gestao/indicadores-e-melhoria.md)
- [Pendências que dependem dos sócios](04-gestao/pendencias-dos-socios.md)
- [Pilotos](05-pilotos/README.md)
