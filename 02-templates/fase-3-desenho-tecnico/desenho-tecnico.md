# Template — Desenho técnico

Descreve **como** a solução atende à especificação. No nível Padrão, preencha as partes 1, 2, 4 (só segurança), 5, 9 e 10. No nível Completo, preencha todas. Os textos entre parênteses orientam o preenchimento.

Dono: Rulian. Revisão de viabilidade: Breno. Fase: [3 — Desenho técnico e plano de tarefas](../../01-fases/fase-3-desenho-tecnico-e-tarefas.md).

| Campo | Preenchimento |
| --- | --- |
| Cliente | |
| Especificação de origem | (título e versão) |
| Responsável | |
| Nível | Leve / Padrão / Completo |
| Status | Rascunho / Revisado pelo Breno / Aprovado |

## 1. Resumo da abordagem

Em poucas linhas, como a solução será construída e por que essa abordagem.

> Escreva aqui.

## 2. Componentes e responsabilidades

| Componente | Responsabilidade | Tecnologia | Por que essa escolha | Requisitos atendidos |
| --- | --- | --- | --- | --- |
| | | | | RF-01 |

## 3. Integrações e contratos

| Sistema externo | Direção (entra ou sai) | Formato e meio | Autenticação | Como trata falha (retentativa) | Responsável |
| --- | --- | --- | --- | --- | --- |
| | | | | | |

## 4. Requisitos não funcionais

| ID | Tipo (desempenho, disponibilidade, segurança, usabilidade, manutenção) | Meta | Como verificar |
| --- | --- | --- | --- |
| RNF-01 | | | |

## 5. Segurança e acesso

| Tema | Definição |
| --- | --- |
| Autenticação e permissões | |
| Guarda de segredos e senhas | |
| Dados pessoais e sob sigilo | |
| Registro de quem fez o quê (auditoria) | |
| Retenção e descarte | |

## 6. Ambientes e implantação

| Ambiente | Para que serve | Onde roda | Quem acessa |
| --- | --- | --- | --- |
| | | | |

## 7. Monitoramento

| O que monitorar | Como | Quem recebe o alerta |
| --- | --- | --- |
| | | |

## 8. Riscos técnicos e decisões

Liste os riscos e os números dos [ADRs](adr.md) relacionados.

> Escreva aqui.

## 9. Cobertura dos requisitos

Cada requisito da especificação precisa aparecer aqui. Esta tabela é a matriz de rastreabilidade da empresa, em versão leve (veja [identificadores e rastreabilidade](../../03-convencoes/identificadores-e-rastreabilidade.md)).

| Requisito | Componente | Tarefa | Teste |
| --- | --- | --- | --- |
| RF-01 | | T-001 | TC-001 |

## 10. Checklist de passagem para a construção

- [ ] Todo requisito tem componente, tarefa e teste
- [ ] Segurança, segredos e acessos estão definidos
- [ ] Decisões relevantes estão registradas em ADR
- [ ] O Breno revisou e confirmou que consegue construir
- [ ] O desenho não contradiz a especificação aprovada

Documentos relacionados: [modelo de dados](modelo-de-dados.md), [ADR](adr.md), [plano de tarefas](plano-de-tarefas.md), [plano de testes](plano-de-testes.md).
