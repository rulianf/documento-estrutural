# 2. Ciclo de vida e portões

O trabalho com cada cliente passa por seis fases. Cada fase tem um dono, produz documentos definidos e só termina quando o **portão** (critério de passagem) é cumprido.

| # | Fase | Dono (apoio) | Entrada | Saída principal | Portão para a próxima fase |
| --- | --- | --- | --- | --- | --- |
| 1 | [Entendimento do negócio](../01-fases/fase-1-entendimento-do-negocio.md) | Lucas (Rulian revisa) | Contato e interesse do cliente | Levantamento da Necessidade | Checklist do levantamento completo: problema, fluxo atual, dores com impacto, linha de base ou plano para obtê-la, decisor e restrições |
| 2 | [Especificação da solução](../01-fases/fase-2-especificacao-da-solucao.md) | Rulian (Lucas valida com o cliente) | Levantamento pronto | Especificação da Solução | Cliente aprovou escopo e critérios de aceite; sócios aprovaram esforço, prazo e investimento |
| 3 | [Desenho técnico e plano de tarefas](../01-fases/fase-3-desenho-tecnico-e-tarefas.md) | Rulian (Breno revisa a viabilidade) | Especificação aprovada | Desenho técnico, modelo de dados, decisões de arquitetura, plano de tarefas e plano de testes | Tarefas pequenas e ligadas aos requisitos; testes ligados aos requisitos; Breno confirma que consegue construir |
| 4 | [Construção](../01-fases/fase-4-construcao.md) | Breno (apoio da IA; Rulian revisa) | Plano de tarefas | Solução construída, testes executados, registro de mudanças | Todas as tarefas concluídas e revisadas; testes passando |
| 5 | [Validação e aceite](../01-fases/fase-5-validacao-e-aceite.md) | Breno executa; Lucas conduz com o cliente; Rulian revisa | Solução construída | Relatório de testes e Registro de entrega e aceite | Cliente aceitou conforme os critérios; sem defeito crítico aberto |
| 6 | [Implantação e operação](../01-fases/fase-6-implantacao-e-operacao.md) | Breno (Lucas cuida do relacionamento) | Entrega aceita | Plano de implantação, runbook, registro de demandas e incidentes | Operação assumida: monitoramento, canal de suporte e classificação de demandas definidos |

**Correspondência com as 5 etapas já definidas:** a etapa 1 (Levantamento) é a fase 1; a etapa 2 (Solução) é a fase 2; a etapa 3 (Arquitetura e tarefas) é a fase 3; a etapa 4 (Construção e entrega) reúne as fases 4 e 5; a etapa 5 (Operação) é a fase 6.

**As fases não são uma esteira rígida.** Se surgir informação nova, volta-se à fase anterior, registra-se o motivo e atualiza-se o documento afetado. Uma mudança de escopo depois da aprovação usa a Solicitação de mudança de escopo (da biblioteca de 15 templates do pacote anterior) e precisa de nova aprovação.

**Antes da fase 4 ninguém constrói nada com compromisso.** Conversa informal não autoriza trabalho relevante: é preciso ter a especificação aprovada.

**Quem aprova** escopo, preço e aceitação do cliente ainda não foi definido pelos sócios (veja [pendências](../04-gestao/pendencias-dos-socios.md)).

Anterior: [princípios e níveis](01-principios-e-niveis.md). Próximo: [catálogo de documentos](03-catalogo-de-documentos.md).
