# Identificadores e rastreabilidade

## Identificadores

Todo item importante recebe um ID que não muda e não é reutilizado. É o que liga o problema do cliente ao requisito, à tarefa, ao teste e ao aceite, e permite entregar à IA só o trecho certo.

| Prefixo | O que identifica | Onde nasce | Exemplo |
| --- | --- | --- | --- |
| RF | Requisito funcional | [Especificação da Solução](../02-templates/fase-2-especificacao/especificacao-da-solucao.md) | RF-01 |
| RN | Regra de negócio | [Especificação da Solução](../02-templates/fase-2-especificacao/especificacao-da-solucao.md) | RN-01 |
| RNF | Requisito não funcional | [Desenho técnico](../02-templates/fase-3-desenho-tecnico/desenho-tecnico.md) | RNF-01 |
| ADR | Decisão de arquitetura | [Registro de decisão](../02-templates/fase-3-desenho-tecnico/adr.md) | ADR-001 |
| T | Tarefa | [Plano de tarefas](../02-templates/fase-3-desenho-tecnico/plano-de-tarefas.md) | T-001 |
| TC | Caso de teste | [Plano de testes](../02-templates/fase-3-desenho-tecnico/plano-de-testes.md) | TC-001 |
| DF | Defeito | [Relatório de testes](../02-templates/fase-5-validacao/relatorio-de-testes.md) | DF-001 |
| DM | Demanda ou incidente | [Registro de demandas](../02-templates/fase-6-operacao/registro-de-demanda-e-incidente.md) | DM-001 |
| F | Fonte do levantamento | [Levantamento da Necessidade](../02-templates/fase-1-levantamento/levantamento-da-necessidade.md) | F1 |

Se um requisito for removido, ele continua na lista com o status **Cancelado** e o motivo, e o ID não é usado de novo.

## Cadeia de rastreabilidade

A cadeia é: **dor do levantamento → requisito (RF, RN) → tarefa (T) → caso de teste (TC) → aceite**. Ela responde às perguntas que mais geram retrabalho.

| Pergunta | Onde está a resposta |
| --- | --- |
| Por que este requisito existe? | Dor citada no requisito, no Levantamento |
| Está construído? | Plano de tarefas, na coluna de requisito |
| Foi testado? | Plano de testes, na coluna de requisito |
| O cliente aceitou? | Registro de entrega e aceite |

A tabela de cobertura do Desenho técnico (parte 9) é a matriz de rastreabilidade da empresa, em versão leve.
