# Template — Plano de testes e casos de teste

Escrito na fase 3, junto com o [desenho técnico](desenho-tecnico.md), e executado nas fases 4 e 5. O resultado da execução vai no [relatório de testes](../fase-5-validacao/relatorio-de-testes.md).

| Campo | Preenchimento |
| --- | --- |
| Cliente | |
| Especificação e desenho de origem | |
| Responsável | |
| Nível | Leve / Padrão / Completo |

## Estratégia

| Tipo de teste | Para que serve | Quando | Quem executa |
| --- | --- | --- | --- |
| Teste de cada parte (unidade) | Conferir regras e cálculos isolados | Durante a construção | Breno, com a IA |
| Teste das partes juntas (integração) | Conferir fluxos e integrações | Fim da construção | Breno |
| Teste de aceite | Conferir os critérios de aceite com dados reais ou amostra combinada | Fase 5 | Cliente, conduzido pelo Lucas |
| Teste de segurança e acesso | Conferir permissões, sigilo e segredos | Antes da entrega | Rulian |

## Dados de teste

Quais dados serão usados, de onde vêm e como se evita expor dados pessoais ou sob sigilo.

> Escreva aqui.

## Casos de teste

| ID | Requisito ou regra | Cenário (dado que, quando, então) | Dados de entrada | Resultado esperado | Tipo (normal ou exceção) | Resultado (passou ou falhou) |
| --- | --- | --- | --- | --- | --- | --- |
| TC-001 | RF-01 | | | | Normal | |

## Regras

Todo requisito funcional e toda regra de negócio têm ao menos um caso normal. Toda exceção listada na especificação tem um caso.

## Critério de saída

Todos os casos essenciais passaram e nenhum defeito crítico ou alto está aberto.
