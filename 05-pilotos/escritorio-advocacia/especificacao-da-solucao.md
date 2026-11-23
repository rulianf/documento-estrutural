# Especificação da Solução — Escritório de Advocacia (piloto)

Preenchida a partir do [levantamento da necessidade](levantamento-da-necessidade.md) do escritório, com o [template](../../02-templates/fase-2-especificacao/especificacao-da-solucao.md). As definições abaixo são **propostas do Rulian** ainda não validadas com a advogada; o que depende dela está marcado como **a confirmar**.

## 1. Identificação, problema e objetivo

| Campo | Preenchimento |
| --- | --- |
| Cliente | Escritório de advocacia da esposa do Lucas |
| Responsável pela especificação | Rulian |
| Levantamento de origem | Levantamento da Necessidade — Escritório de Advocacia (piloto) |
| Status | Rascunho |

**Problema:** a advogada não tem uma visão organizada do que foi combinado com cada cliente, do que já recebeu e do que está em atraso (dor 1, a principal segundo o Lucas), e perde tempo com tarefas administrativas que a afastam da petição (dor 3). Os contratos e documentos estão soltos em pastas desorganizadas (dor 4), e não existe nenhum número de hoje para medir melhora.

**Objetivo da fase 1:** organizar em uma base única os casos, os contratos de honorários e os pagamentos, de modo que a advogada veja a qualquer momento o que tem a receber, o que recebeu e o que está atrasado, e que o escritório passe a ter a linha de base que falta (volume de casos, valores em aberto, inadimplência e tempo administrativo). A meta numérica será definida depois que essa linha de base existir.

Esta fase não tenta resolver as dores 2 e 5 nem gerar documentos automaticamente. Isso fica para fases seguintes.

## 2. Escopo e processo futuro

**Escopo da fase 1**

| Incluído nesta entrega | Excluído desta entrega | Fica para depois |
| --- | --- | --- |
| Cadastro de casos com a etapa em que cada um está | Gravação das reuniões e geração automática de contrato, procuração e petição | Gravar a reunião de fechamento e extrair os dados dela |
| Cadastro dos contratos de honorários, com a forma de remuneração de cada cliente | Integração com o WhatsApp | Gerar rascunhos de proposta, contrato e petição para aprovação |
| Cadastro dos pagamentos previstos e recebidos de cada contrato | Tela de consulta do cliente | Atendimento automático de perguntas sobre andamento |
| Carga inicial a partir dos contratos nas pastas e do extrato bancário | Acompanhamento de prazos e audiências | Cobrança de documentos faltantes pelo WhatsApp |
| Visão do que há a receber, do que foi recebido e do que está em atraso | Ligação com a assinatura eletrônica e com o banco | Controle de tarefas por caso e acompanhamento de prazos |
| Lista de pendências (contrato sem assinatura, sem arquivo, parcela vencida) | | |

**Usuários e papéis**

| Quem | O que faz na solução | Permissões |
| --- | --- | --- |
| Advogada | Confere os dados carregados, registra e consulta casos, contratos e pagamentos | Ver e alterar tudo |
| Lucas e Rulian | Fazem a carga inicial e dão suporte | A confirmar com a advogada, com acesso mínimo necessário |

**Processo futuro (TO-BE) nesta fase:** só mudam as etapas ligadas a contrato e pagamento. As demais continuam como hoje.

| Etapa do fluxo atual | O que muda | Tipo de mudança | Continua manual? |
| --- | --- | --- | --- |
| 4. Contrato e procuração | O modelo de remuneração e as datas passam a ser registrados no cadastro | Padronizada | Sim: a advogada continua redigindo |
| 5. Assinatura | Registrar se o contrato foi assinado e guardar o arquivo assinado na pasta | Padronizada | Sim |
| 6. Entrada financeira | O caso só é marcado como pronto para a petição depois de registrada a entrada, quando o contrato a prevê | Padronizada | Sim: o registro é feito à mão |
| 10. Cobrança dos honorários | O que vence, o que foi pago e o que está em atraso fica visível em um só lugar | Simplificada | Sim: a cobrança em si continua com a advogada |
| Demais etapas (contato, reunião, proposta, documentos, petição, acompanhamento) | Sem mudança nesta fase | Nenhuma | Sim |

**Pontos de decisão e revisão humana:** a advogada confere os dados lidos de cada contrato antes de eles valerem no cadastro, e decide sozinha sobre cobrança e contato com clientes.

## 3. Requisitos e regras

**Requisitos funcionais**

| ID | Requisito | Dor (nº) | Prioridade | Critério de aceite |
| --- | --- | --- | --- | --- |
| RF-01 | Registrar cada cliente e caso, com tipo de ação, data de início e etapa atual | 3, 4 | Essencial | Todos os casos ativos aparecem listados, cada um com sua etapa |
| RF-02 | Registrar o contrato de honorários de cada caso: modelo de remuneração, percentual ou valor, datas de vencimento e se está assinado | 1 | Essencial | Para qualquer caso, é possível ver o modelo de remuneração e se há contrato assinado |
| RF-03 | Registrar os pagamentos de um contrato, previstos e recebidos, com data, valor e tipo (entrada, parcela ou êxito) | 1 | Essencial | Um contrato com entrada e três parcelas mostra os quatro pagamentos e o que já foi pago |
| RF-04 | Calcular, por contrato e no total, o valor previsto, o recebido, o em aberto e o em atraso | 1 | Essencial | Os totais batem com a conferência manual de uma amostra de contratos escolhida com a advogada |
| RF-05 | Carga inicial dos casos e contratos existentes, lendo as pastas do Drive | 1, 4 | Essencial | Todos os clientes das pastas foram carregados, e a advogada conferiu os dados de cada contrato |
| RF-06 | Marcar o status do caso pela regra da entrada: aguardando assinatura, aguardando entrada, pronto para a petição ou em andamento | 3 | Importante | O status de cada caso confere com a regra RN-01 e RN-02 |
| RF-07 | Conciliar os pagamentos recebidos com o extrato bancário do período | 1 | Importante | Cada pagamento do extrato fica ligado a um contrato, ou marcado como não identificado |
| RF-08 | Listar pendências: contrato sem assinatura registrada, caso sem contrato salvo e parcela vencida | 1, 4 | Importante | A lista reúne todos os casos nessas situações, sem omitir nenhum da amostra conferida |
| RF-09 | Registrar o tempo gasto em tarefas administrativas por semana, para a linha de base | 3 | Desejável | A advogada consegue lançar o tempo em menos de um minuto por dia |

**Regras de negócio** (propostas a partir da conversa entre Lucas e Rulian)

| ID | Regra | Origem | Confirmada pelo cliente? |
| --- | --- | --- | --- |
| RN-01 | Sem contrato assinado não existe caso em andamento: o caso fica aguardando assinatura | Relato do Lucas | A confirmar |
| RN-02 | Se o contrato prevê entrada, a petição inicial só começa depois do pagamento da entrada; se não prevê, segue direto | Relato do Lucas | A confirmar |
| RN-03 | Um contrato pode ter vários pagamentos, e a entrada é um tipo de pagamento | Rulian | A confirmar |
| RN-04 | Em contrato só no êxito, nada é devido antes do resultado, e o valor é um percentual do proveito econômico | Relato do Lucas | A confirmar |
| RN-05 | Percentuais e valores variam por cliente: cada contrato guarda os seus | Relato do Lucas | A confirmar |
| RN-06 | Um pagamento com data prevista já passada e sem recebimento está em atraso; pagamento ligado ao êxito não entra em atraso antes do resultado | Proposta do Rulian | A confirmar |

**Exceções e erros**

| Situação | Como a solução se comporta |
| --- | --- |
| Contrato assinado que não está na pasta | Aparece na lista de pendências até o arquivo ser guardado |
| Contrato ilegível ou sem a forma de remuneração clara | Não entra no cadastro até a advogada informar os dados |
| Pagamento do extrato sem contrato identificável | Fica como não identificado até a advogada indicar o cliente |
| Pagamento parcial | Registra o valor recebido e mantém o restante em aberto |
| Percentual ou valor alterado depois da assinatura | Guarda o valor atual e o anterior, com a data da mudança |

## 4. Dados, segurança, dependências e riscos

**Dados de entrada e saída**

| Dado ou documento | Entra ou sai | De onde vem ou para onde vai | Formato | Quem fornece |
| --- | --- | --- | --- | --- |
| Contratos de honorários e procurações | Entra | Pastas dos clientes no Drive | Word ou PDF | Advogada |
| Extrato bancário do período | Entra | Banco da advogada | A confirmar | Advogada |
| Dados do caso (tipo de ação, data de início, etapa) | Entra | Informados pela advogada | A definir | Advogada |
| Tempo administrativo por semana | Entra | Lançado pela advogada | A definir | Advogada |
| Lista de casos com etapa e status | Sai | Para a advogada | A definir no desenho técnico | Solução |
| Total previsto, recebido, em aberto e em atraso | Sai | Para a advogada | A definir no desenho técnico | Solução |
| Lista de pendências | Sai | Para a advogada | A definir no desenho técnico | Solução |

**Segurança, privacidade e revisão humana**

| Tema | Definição |
| --- | --- |
| Dados pessoais ou sensíveis tratados | Nomes, documentos e dados de processos dos clientes (LGPD) e informações sob sigilo profissional da advocacia |
| Quem pode ver e alterar | A advogada; Lucas e Rulian só com acesso mínimo necessário (a confirmar) |
| Uso de IA sobre esses dados | **A confirmar com a advogada.** Nenhum documento de cliente é enviado a ferramenta de IA antes dessa autorização |
| O que uma pessoa precisa revisar antes de valer | Os dados lidos de cada contrato, pela advogada |
| Retenção e descarte | **Não definido** |

**Integrações e dependências**

| Item | Quem fornece | Para quando |
| --- | --- | --- |
| Acesso às pastas dos clientes no Drive | Advogada | Antes da carga inicial |
| Extrato bancário do período | Advogada | Antes da conciliação |
| Autorização para tratar os dados e, se for o caso, usar IA | Advogada | Antes da carga inicial |
| Tempo da advogada para conferir a carga | Advogada | A definir |

**Premissas e restrições:** nesta fase não há infraestrutura em nuvem nem integração com outros sistemas; a base pode ser simples e local, e a tecnologia será escolhida no desenho técnico. O WhatsApp continua sendo o canal com os clientes. Todos os casos ativos têm contrato guardado em alguma pasta (a verificar).

**Riscos**

| Risco | Probabilidade e impacto | O que fazer |
| --- | --- | --- |
| Contratos ausentes ou ilegíveis nas pastas | Alta, com impacto médio na carga | Listar como pendência e pedir o arquivo à advogada |
| Pastas desorganizadas tornam a carga mais lenta que o previsto | Alta, com impacto médio no prazo | Medir o esforço nos primeiros casos antes de prometer prazo |
| Extrato sem identificação do cliente em cada pagamento | Média, com impacto médio na conciliação | Conferir com a advogada os pagamentos não identificados |
| Dados sigilosos tratados sem autorização | Baixa, com impacto alto | Não carregar nada antes da autorização e do acesso mínimo definido |
| Advogada sem tempo para conferir a carga | Média, com impacto alto na qualidade | Combinar horários curtos e fixos de conferência |

## 5. Aceite, validação e medição

**Plano de validação**

| Etapa de validação | O que será conferido | Quem confere | Quando |
| --- | --- | --- | --- |
| Primeiros casos carregados | Os dados lidos de cada contrato estão corretos | Advogada | Logo após a carga dos primeiros casos |
| Totais | Previsto, recebido, em aberto e em atraso de uma amostra de contratos batem com a conta manual | Advogada e Rulian | Depois da carga completa |
| Pendências | A lista cobre todos os casos sem contrato salvo ou sem assinatura registrada | Advogada | Depois da carga completa |
| Uso real | A advogada consulta o cadastro no dia a dia e informa o que falta | Advogada | Nas primeiras semanas de uso |

O tamanho da amostra e as datas serão combinados com a advogada.

**Medição do resultado**

| Medida | Valor hoje (linha de base) | Meta | Como e quando será medida |
| --- | --- | --- | --- |
| Casos ativos e novos por mês | Não existe | A definir após a linha de base | Contagem a partir do cadastro, todo mês |
| Tempo administrativo por semana | Não existe | A definir após a linha de base | Lançamento semanal da advogada (RF-09) |
| Valor em aberto ou atrasado | Não existe | A definir após a linha de base | Totais do cadastro (RF-04), todo mês |
| Taxa de inadimplência | Não existe | A definir após a linha de base | Valor em atraso sobre o previsto, todo mês |
| Casos parados por falta de documento ou assinatura | Não existe | A definir após a linha de base | Lista de pendências (RF-08) |

**Condição de aceite final:** a advogada confirma que o cadastro reflete os casos e contratos reais, os totais conferem com a amostra validada e a linha de base está registrada. A meta de melhoria será combinada com ela só depois disso.

## 6. Pendências, aprovação e checklist de passagem

**Pendências**

| Pendência | Quem resolve | Prazo |
| --- | --- | --- |
| Confirmar com a advogada as regras RN-01 a RN-06 | Lucas | A definir |
| Autorização para tratar os dados e, se for o caso, usar IA | Advogada | A definir |
| Definir quem acessa os dados e com que permissão | Rulian e advogada | A definir |
| Definir retenção e descarte dos dados | Rulian | A definir |
| Quantidade de casos ativos, para estimar o esforço da carga | Lucas | A definir |
| Forma de pagamento dos clientes e onde ela confere os recebimentos | Lucas | A definir |
| Definir quem aprova escopo, preço e aceite do cliente | Sócios | A definir |
| Estimar esforço, prazo e custo da fase 1 | Rulian | Depois do número de casos |

**Aprovação**

| Quem aprova | Parte aprovada | Data |
| --- | --- | --- |
| Advogada | Escopo e critérios de aceite | Pendente |
| Sócios | Esforço, prazo e investimento ou capacidade | Pendente |

**Checklist de passagem para o desenho técnico.** Itens desmarcados ainda impedem o envio.

- [x] O problema e o objetivo estão ligados às dores do levantamento
- [x] Escopo, exclusões e itens para depois estão definidos
- [x] Cada etapa do fluxo atual foi avaliada: eliminar, simplificar, padronizar ou automatizar
- [x] Todo requisito tem prioridade e critério de aceite
- [ ] As regras de negócio foram confirmadas pelo cliente
- [ ] Dados, segurança e revisão humana estão definidos
- [x] Dependências, premissas e riscos estão registrados
- [x] Existe plano de validação e medição contra a linha de base
- [ ] O cliente aprovou o escopo e os critérios de aceite
- [x] As pendências estão listadas com responsável
