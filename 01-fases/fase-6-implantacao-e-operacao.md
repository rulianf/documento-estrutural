# Fase 6 — Implantação e operação

| Item | Conteúdo |
| --- | --- |
| Objetivo | Colocar a solução em uso, transferi-la para a operação e mantê-la, corrigi-la e evoluí-la |
| Responsável | Breno implanta e opera; Lucas cuida do relacionamento e das expectativas; Rulian decide sobre mudanças relevantes |
| Entradas | Entrega aceita |
| Atividades | Implantar conforme o plano, com a reversão pronta; orientar o usuário com um guia rápido; definir monitoramento, canal e horário de suporte; receber e classificar cada demanda; corrigir incidentes e comunicar o cliente; rever periodicamente o resultado contra a linha de base; levar melhorias maiores e projetos novos de volta à fase 1 ou 2 |
| Documentos | [Plano de implantação e reversão](../02-templates/fase-6-operacao/plano-de-implantacao-e-reversao.md); [Runbook](../02-templates/fase-6-operacao/runbook.md) (nível Completo); guia rápido; [Registro de demandas e incidentes](../02-templates/fase-6-operacao/registro-de-demanda-e-incidente.md); registro de mudanças |
| Portão | Operação assumida: monitoramento e canal de suporte definidos, runbook entregue quando exigido, cliente sabe como pedir ajuda e a primeira demanda foi classificada pelo processo |
| Erros comuns | Contrato recorrente sem limite de capacidade nem de escopo; misturar incidente com melhoria; implantar sem plano de reversão; não medir o resultado depois da entrega; operação que depende de uma só pessoa |
| Papel da IA | Classificar e resumir demandas, sugerir causa provável a partir de logs, rascunhar comunicação ao cliente e atualizar o runbook. Comunicação crítica e decisões passam por revisão humana |

## Classificação de demandas na operação

Toda demanda recebida é classificada antes de qualquer trabalho.

| Tipo | O que é | Para onde vai |
| --- | --- | --- |
| Incidente | Algo que funcionava deixou de funcionar | Correção imediata, dentro da operação |
| Suporte | Dúvida de uso ou pedido que não altera o sistema | Atendimento na operação |
| Melhoria | Ajuste ou ampliação do que já existe | Avaliação e priorização; se for grande, vira projeto |
| Projeto novo | Novo escopo, módulo ou integração relevante | Volta à [fase 1](fase-1-entendimento-do-negocio.md) ou [2](fase-2-especificacao-da-solucao.md) |

Fase anterior: [validação e aceite](fase-5-validacao-e-aceite.md).
