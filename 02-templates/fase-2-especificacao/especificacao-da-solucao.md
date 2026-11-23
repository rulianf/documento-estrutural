# Template — Especificação da Solução

Use este template para transformar o levantamento da necessidade em uma intervenção específica: **o que a solução precisa fazer**, sem dizer como será construída. A escolha de tecnologia e a arquitetura ficam no desenho técnico, na etapa seguinte.

Dono: Rulian. Validação com o cliente: Lucas. Fase: [2 — Especificação da solução](../../01-fases/fase-2-especificacao-da-solucao.md).

## 1. Identificação, problema e objetivo

| Campo | Preenchimento |
| --- | --- |
| Cliente | |
| Responsável pela especificação | |
| Levantamento de origem | Título do documento de levantamento da necessidade |
| Status | Rascunho / Em revisão / Aprovada pelo cliente |

**Problema:** qual é o problema que esta solução resolve? Resuma em poucas linhas e cite o número das dores do levantamento que ela ataca.

> Escreva aqui.

**Objetivo:** que resultado mensurável o cliente terá? Use as medidas da linha de base do levantamento.

> Escreva aqui.

## 2. Escopo e processo futuro

Antes de automatizar, pergunte para cada etapa do fluxo atual: ela pode ser eliminada, simplificada ou padronizada? Só o que sobrar vira solução.

**Escopo**

| Incluído nesta entrega | Excluído desta entrega | Fica para depois |
| --- | --- | --- |
| | | |

**Usuários e papéis**

| Quem | O que faz na solução | Permissões |
| --- | --- | --- |
| | | |

**Processo futuro (TO-BE):** compare com o fluxo atual do levantamento, só nas etapas que mudam.

| Etapa do fluxo atual | O que muda | Tipo de mudança (eliminada, simplificada, padronizada, automatizada) | Continua manual? |
| --- | --- | --- | --- |
| | | | |

**Pontos de decisão e revisão humana:** onde uma pessoa precisa aprovar antes de o processo seguir?

> Escreva aqui.

## 3. Requisitos e regras

Escreva o que a solução faz, não como. Cada requisito precisa de um critério de aceite que alguém consiga verificar com sim ou não.

**Requisitos funcionais**

| ID | Requisito | Dor (nº) | Prioridade (Essencial, Importante, Desejável) | Critério de aceite |
| --- | --- | --- | --- | --- |
| RF-01 | | | | |
| RF-02 | | | | |

**Regras de negócio:** regras do cliente que a solução precisa respeitar.

| ID | Regra | Origem (quem definiu) | Confirmada pelo cliente? |
| --- | --- | --- | --- |
| RN-01 | | | |

**Exceções e erros:** o que acontece quando algo foge do normal?

| Situação | Como a solução se comporta |
| --- | --- |
| | |

## 4. Dados, segurança, dependências e riscos

**Dados de entrada e saída**

| Dado ou documento | Entra ou sai | De onde vem ou para onde vai | Formato | Quem fornece |
| --- | --- | --- | --- | --- |
| | | | | |

**Segurança, privacidade e revisão humana**

| Tema | Definição |
| --- | --- |
| Dados pessoais ou sensíveis tratados | |
| Quem pode ver e alterar | |
| Uso de IA sobre esses dados (autorizado por quem?) | |
| O que uma pessoa precisa revisar antes de valer | |
| Retenção e descarte | |

**Integrações e dependências:** sistemas, acessos e pessoas de que a entrega depende.

| Item | Quem fornece | Para quando |
| --- | --- | --- |
| | | |

**Premissas e restrições:** o que estamos assumindo como verdadeiro e o que não pode mudar.

> Escreva aqui.

**Riscos**

| Risco | Probabilidade e impacto | O que fazer |
| --- | --- | --- |
| | | |

## 5. Aceite, validação e medição

**Plano de validação:** como o cliente vai conferir que a solução faz o que foi especificado?

| Etapa de validação | O que será conferido | Quem confere | Quando |
| --- | --- | --- | --- |
| | | | |

**Medição do resultado:** compare com a linha de base do levantamento.

| Medida | Valor hoje (linha de base) | Meta | Como e quando será medida |
| --- | --- | --- | --- |
| | | | |

**Condição de aceite final:** o que precisa ser verdade para o cliente dar a entrega como concluída?

> Escreva aqui.

## 6. Pendências, aprovação e checklist de passagem

**Pendências:** decisões ou informações que ainda faltam, com responsável. Não invente respostas: registre aqui.

| Pendência | Quem resolve | Prazo |
| --- | --- | --- |
| | | |

**Aprovação**

| Quem aprova | Parte aprovada | Data |
| --- | --- | --- |
| Cliente | Escopo e critérios de aceite | |
| Sócios | Esforço, prazo e investimento ou capacidade | |

**Checklist de passagem para o desenho técnico.** Só envie ao desenho técnico quando todos os itens estiverem marcados.

- [ ] O problema e o objetivo estão ligados às dores do levantamento
- [ ] Escopo, exclusões e itens para depois estão definidos
- [ ] Cada etapa do fluxo atual foi avaliada: eliminar, simplificar, padronizar ou automatizar
- [ ] Todo requisito tem prioridade e critério de aceite
- [ ] As regras de negócio foram confirmadas pelo cliente
- [ ] Dados, segurança e revisão humana estão definidos
- [ ] Dependências, premissas e riscos estão registrados
- [ ] Existe plano de validação e medição contra a linha de base
- [ ] O cliente aprovou o escopo e os critérios de aceite
- [ ] As pendências estão listadas com responsável

Exemplo preenchido: [piloto do escritório de advocacia](../../05-pilotos/escritorio-advocacia/especificacao-da-solucao.md).
