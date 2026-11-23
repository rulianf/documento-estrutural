# Fase 4 — Construção

| Item | Conteúdo |
| --- | --- |
| Objetivo | Construir a solução conforme a especificação e o desenho, com qualidade, segurança e rastreabilidade |
| Responsável | Breno constrói, com apoio da IA; Rulian revisa o que for entregue (proposta, a confirmar entre os sócios) |
| Entradas | [Plano de tarefas](../02-templates/fase-3-desenho-tecnico/plano-de-tarefas.md), Desenho técnico, Especificação e [arquivo de contexto para a IA](../03-convencoes/contexto-para-ia/contexto-da-empresa.md) |
| Atividades | Para cada tarefa, dar à IA só o contexto relevante: o trecho da especificação, o do desenho e o ID da tarefa; implementar; escrever e executar os testes ligados aos requisitos; revisar o código antes de integrar; registrar as mudanças; atualizar a especificação ou o desenho quando uma decisão mudar durante a construção; versionar tudo |
| Documentos | Código e scripts no repositório; README; registro de mudanças; testes executados; especificação e desenho atualizados |
| Portão | Todas as tarefas concluídas e revisadas; testes passando; documentação atualizada |
| Erros comuns | Pedir à IA para reescrever grandes partes sem especificação; integrar código gerado que ninguém revisou; mudar comportamento sem atualizar a especificação; guardar segredos no repositório; carregar o repositório inteiro como contexto |
| Papel da IA | Gerar código e testes, explicar trechos, refatorar dentro do escopo e ajudar na revisão. A IA não decide mudança de escopo nem de arquitetura |

Esta fase não tem template próprio: o resultado é código no repositório do cliente.

Fase anterior: [desenho técnico e tarefas](fase-3-desenho-tecnico-e-tarefas.md). Próxima fase: [validação e aceite](fase-5-validacao-e-aceite.md).
