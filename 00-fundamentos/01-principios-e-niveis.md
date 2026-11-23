# 1. Princípios e níveis de formalização

A engenharia clássica produzia muitos documentos para controlar projetos longos e contratos por escopo fechado. A empresa mantém a **separação de camadas** que ela criou, mas ajusta a profundidade ao tamanho de cada trabalho.

## Princípios

- **Documentar para decidir, construir, validar e manter.** Se um documento não ajuda nenhuma dessas quatro coisas, não é produzido.
- **Três camadas separadas:** negócio (qual problema), solução (o que o sistema faz) e implementação (como é construído). Cada uma responde a perguntas diferentes e fica em documento próprio.
- **A profundidade acompanha o risco**, e não o tamanho do cliente. Dados sensíveis, dinheiro e integração com outros sistemas pedem mais documentação.
- **A especificação é a fonte de referência** para pessoas e para a IA. Quando o sistema muda, a especificação muda junto.
- **Identificadores ligam tudo.** Um requisito (RF-03) aparece na tarefa, no teste e no aceite, para que nada seja esquecido nem inventado. Veja [identificadores e rastreabilidade](../03-convencoes/identificadores-e-rastreabilidade.md).
- **Nada começa sem portão.** Cada fase só começa quando o critério de passagem da anterior está cumprido.
- **A IA apoia; pessoas decidem.** Aprovação, segurança e qualidade continuam humanas.
- **Pendência é registrada, não preenchida com suposição.** Campo sem resposta recebe "não informado" ou "a confirmar".

## O que foi mantido, simplificado e cortado da engenharia clássica

| Tratamento | O que é |
| --- | --- |
| Mantido | Entendimento do negócio antes dos requisitos, especificação de requisitos, regras de negócio, modelo de dados, arquitetura, plano de testes, termo de aceite, plano de implantação e reversão |
| Simplificado | Casos de uso viram cenários curtos; UML vira três diagramas essenciais (fluxo, dados e componentes); rastreabilidade vira IDs padronizados; manuais viram runbook de uma página |
| Cortado por enquanto | Business case formal, contagem por Ponto de Função, matriz de rastreabilidade completa, diagramas UML de sequência, de classes e de estados fora de casos complexos, manual do usuário extenso |

## Níveis de formalização

Cada trabalho recebe um nível no início, e o nível define quais documentos são exigidos. Os critérios abaixo são uma proposta para ser ajustada com a experiência do piloto.

| Nível | Quando usar | Documentos exigidos |
| --- | --- | --- |
| Leve | Melhoria pequena, baixo risco, reversível, sem dados pessoais nem dinheiro | Ficha de demanda (problema, resultado esperado, aceite) e registro de entrega |
| Padrão | Nova funcionalidade ou automação com regra de negócio, integração simples, dados do cliente | Levantamento da necessidade, especificação da solução, desenho técnico curto, plano de tarefas, plano de testes e registro de entrega e aceite |
| Completo | Sistema novo, integração com sistemas externos ou financeiros, dados sensíveis ou sob sigilo, alto impacto no cliente | Todos os documentos do Padrão, mais modelo de dados, decisões de arquitetura (ADR), plano de implantação e reversão e runbook |

O piloto do escritório de advocacia entra como **Padrão, com atenção reforçada a LGPD e sigilo profissional** (proposta). Se a fase seguinte incluir integração com WhatsApp, assinatura eletrônica ou banco, o nível sobe para Completo.

Próximo: [ciclo de vida e portões](02-ciclo-de-vida-e-portoes.md).
