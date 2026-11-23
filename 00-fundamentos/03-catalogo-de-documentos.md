# 3. Catálogo de documentos

A tabela mostra cada documento da engenharia clássica, a versão que a empresa adota, a fase em que aparece e o **nível mínimo** que o exige (a partir de Leve, Padrão ou Completo). A coluna "Template" aponta para o arquivo; "Sob demanda" significa que não há template fixo e o documento só é feito quando o caso pede.

| Documento clássico | Versão adotada | Fase | Nível mínimo | Template |
| --- | --- | --- | --- | --- |
| Documento de visão do negócio | Resumo e contexto do Levantamento | 1 | Padrão | [Levantamento](../02-templates/fase-1-levantamento/levantamento-da-necessidade.md) |
| Business Case | Resultado esperado e linha de base do Levantamento; estudo formal só se o cliente pedir | 1 | Completo | [Levantamento](../02-templates/fase-1-levantamento/levantamento-da-necessidade.md) (seção 5) |
| BRD (levantamento do negócio) | Levantamento da Necessidade | 1 | Padrão | [Levantamento](../02-templates/fase-1-levantamento/levantamento-da-necessidade.md) |
| Mapeamento AS-IS | Tabela do fluxo atual; BPMN só quando o fluxo for complexo ou crítico | 1 | Padrão | [Levantamento](../02-templates/fase-1-levantamento/levantamento-da-necessidade.md) (seção 2) |
| Análise de stakeholders | Contexto, decisores e usuários do Levantamento | 1 | Padrão | [Levantamento](../02-templates/fase-1-levantamento/levantamento-da-necessidade.md) (seção 2) |
| Regras de negócio | Tabela de regras (RN) da Especificação | 2 | Padrão | [Especificação](../02-templates/fase-2-especificacao/especificacao-da-solucao.md) (seção 3) |
| Definição de escopo | Escopo incluído, excluído e para depois, na Especificação | 2 | Leve | [Especificação](../02-templates/fase-2-especificacao/especificacao-da-solucao.md) (seção 2) |
| Mapeamento TO-BE | Processo futuro na Especificação | 2 | Padrão | [Especificação](../02-templates/fase-2-especificacao/especificacao-da-solucao.md) (seção 2) |
| ERS / SRS | Especificação da Solução | 2 | Padrão | [Especificação](../02-templates/fase-2-especificacao/especificacao-da-solucao.md) |
| Requisitos funcionais | Tabela de RF com prioridade e critério de aceite | 2 | Leve | [Especificação](../02-templates/fase-2-especificacao/especificacao-da-solucao.md) (seção 3) |
| Requisitos não funcionais | Segurança na Especificação; desempenho, disponibilidade e usabilidade no Desenho técnico (RNF) | 2 e 3 | Padrão | [Especificação](../02-templates/fase-2-especificacao/especificacao-da-solucao.md) e [Desenho técnico](../02-templates/fase-3-desenho-tecnico/desenho-tecnico.md) |
| Casos de uso | Cenários curtos, escritos como critérios de aceite | 2 | Completo | Sob demanda |
| Especificação de interfaces | Contratos de integração no Desenho técnico | 3 | Completo | [Desenho técnico](../02-templates/fase-3-desenho-tecnico/desenho-tecnico.md) (parte 3) |
| Matriz de rastreabilidade | IDs padronizados e coluna de requisito no Plano de tarefas | 3 | Padrão | [Identificadores e rastreabilidade](../03-convencoes/identificadores-e-rastreabilidade.md) |
| Glossário | Glossário no arquivo de contexto para a IA | 2 | Padrão | [Contexto do cliente](../03-convencoes/contexto-para-ia/contexto-do-cliente.md) |
| Documento de arquitetura e especificação técnica | Desenho técnico | 3 | Padrão (versão curta) | [Desenho técnico](../02-templates/fase-3-desenho-tecnico/desenho-tecnico.md) |
| Modelo conceitual, lógico e físico de dados | Modelo de dados: entidades, atributos e relações; físico só no nível Completo | 3 | Padrão | [Modelo de dados](../02-templates/fase-3-desenho-tecnico/modelo-de-dados.md) |
| Diagramas UML | Três diagramas essenciais: fluxo, dados e componentes | 3 | Completo | [Modelo de dados](../02-templates/fase-3-desenho-tecnico/modelo-de-dados.md) e [Desenho técnico](../02-templates/fase-3-desenho-tecnico/desenho-tecnico.md) |
| Protótipos de tela | Esboço das telas, só quando houver interface | 3 | Padrão | Sob demanda |
| Registro de decisão de arquitetura (ADR) | ADR | 3 | Completo | [ADR](../02-templates/fase-3-desenho-tecnico/adr.md) |
| Diagrama de implantação | Seção de ambientes no Desenho técnico | 3 | Completo | [Desenho técnico](../02-templates/fase-3-desenho-tecnico/desenho-tecnico.md) (parte 6) |
| Backlog e tarefas de implementação | Plano de tarefas ligado aos RF | 3 | Padrão | [Plano de tarefas](../02-templates/fase-3-desenho-tecnico/plano-de-tarefas.md) |
| Código, scripts e documentação de API | Repositório com README e contratos de API | 4 | Leve | No repositório de código |
| Registro de versões e mudanças | Registro de mudanças no repositório | 4 | Padrão | No repositório de código |
| Plano de testes | Plano de testes | 3 | Padrão | [Plano de testes](../02-templates/fase-3-desenho-tecnico/plano-de-testes.md) |
| Casos de teste | Tabela de casos ligados aos RF | 3 | Padrão | [Plano de testes](../02-templates/fase-3-desenho-tecnico/plano-de-testes.md) |
| Evidências e relatório de defeitos | Relatório de testes com evidências e defeitos | 5 | Padrão | [Relatório de testes](../02-templates/fase-5-validacao/relatorio-de-testes.md) |
| Termo de homologação e de aceite | Registro de entrega e aceite | 5 | Leve | [Registro de entrega e aceite](../02-templates/fase-5-validacao/registro-de-entrega-e-aceite.md) |
| Plano de implantação e de rollback | Plano de implantação e reversão | 6 | Completo | [Plano de implantação](../02-templates/fase-6-operacao/plano-de-implantacao-e-reversao.md) |
| Manual do usuário | Guia rápido de uma página | 6 | Padrão | Sob demanda |
| Manual operacional e runbook | Runbook | 6 | Completo | [Runbook](../02-templates/fase-6-operacao/runbook.md) |
| Documentação de infraestrutura | Seção de ambientes e registro de acessos | 6 | Completo | [Desenho técnico](../02-templates/fase-3-desenho-tecnico/desenho-tecnico.md) (parte 6) |
| Documentação de manutenção | Registro de demandas e incidentes | 6 | Padrão | [Registro de demanda e incidente](../02-templates/fase-6-operacao/registro-de-demanda-e-incidente.md) |

Anterior: [ciclo de vida e portões](02-ciclo-de-vida-e-portoes.md).
