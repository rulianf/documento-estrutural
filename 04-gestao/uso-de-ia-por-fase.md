# Uso de IA por fase

| Fase | A IA pode | A pessoa decide | Cuidado |
| --- | --- | --- | --- |
| 1. Entendimento do negócio | Transcrever e resumir entrevistas, organizar o relato no template, apontar lacunas | Lucas valida o conteúdo com o cliente | Dados sob sigilo só com autorização do cliente |
| 2. Especificação | Rascunhar requisitos e critérios de aceite, achar contradições | Rulian aprova o escopo; o cliente aprova | Enviar só o levantamento relevante |
| 3. Desenho técnico | Propor alternativas com prós e contras, rascunhar modelo de dados e tarefas | Rulian decide a arquitetura | Pedir que cite os IDs cobertos |
| 4. Construção | Gerar código e testes, explicar e refatorar dentro do escopo | Breno e Rulian revisam; nada é integrado sem revisão humana | Contexto por tarefa, nunca o repositório inteiro |
| 5. Validação | Gerar casos de teste, apontar requisito sem teste, resumir resultados | O cliente aceita | Não aceitar resultado sem evidência |
| 6. Operação | Classificar e resumir demandas, sugerir causa a partir de logs, rascunhar comunicação | Pessoa aprova toda comunicação crítica | Segredos e dados de cliente fora dos pedidos |

## Custo total, não só custo de geração

A decisão sobre quanto documentar considera tokens, tempo humano, retrabalho, risco e manutenção. Documento longo ou desatualizado consome contexto e induz erro; documento ausente faz a IA inventar decisões. A meta é o menor custo ao longo de todo o ciclo de vida.

Regras gerais de comportamento da IA: [contexto da empresa](../03-convencoes/contexto-para-ia/contexto-da-empresa.md).
