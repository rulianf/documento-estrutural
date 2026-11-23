# Pastas por cliente

Todo cliente tem a mesma estrutura, para que qualquer sócio e a IA encontrem o documento certo.

| Pasta | Conteúdo |
| --- | --- |
| 00-Contexto | [Contexto para a IA](contexto-para-ia/contexto-do-cliente.md), glossário e lista de acessos (sem senhas) |
| 01-Levantamento | Levantamento da Necessidade e materiais de apoio |
| 02-Especificacao | Especificação da Solução e solicitações de mudança de escopo |
| 03-Desenho-tecnico | Desenho técnico, modelo de dados, ADRs, plano de tarefas e plano de testes |
| 04-Construcao | Ponteiro para o repositório de código |
| 05-Validacao-e-aceite | Relatório de testes e Registro de entrega e aceite |
| 06-Operacao | Plano de implantação, runbook e registro de demandas e incidentes |
| 99-Historico | Versões substituídas |

## Nome dos arquivos

Padrão: **Tipo - Cliente - vX.Y**. Exemplo: `Especificação - Escritório piloto - v1.0`.

No repositório Git, prefira nomes em minúsculas, sem acento e com hífens (por exemplo, `especificacao-escritorio-piloto-v1.0.md`), mantendo o tipo e a versão no nome.

## Atenção a dados de cliente

Documentos de cliente trazem dados pessoais e, em alguns casos, informação sob sigilo profissional. **Não suba documentos reais de clientes para um repositório público.** Este repositório guarda o método e os templates; as pastas de clientes devem ficar em repositório privado com acesso mínimo necessário.
