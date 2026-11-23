# Atalho: Planejador Semanal de Estudos

Use no início de cada semana para transformar o tempo disponível num plano que pode ser conferido. Adaptado de [Bom Pedido](../02-templates/01-bom-prompt.md) e [Preparar uma Reunião](../01-prompts/05-preparar-reuniao.md).

## Modelo

Copie o bloco, troque apenas o que está entre `{{ }}` e cole na IA que você usa.

```text
CONTEXTO
Sou estudante de desenvolvimento e estou organizando a semana de {{semana}}.
Tenho {{horas_totais}} disponíveis em {{quantidade_blocos}} blocos: {{dias_e_horarios}}.
Foco atual: {{trilha_de_estudo}}.
Já adaptei meus prompts e checklists e quero equilibrar teoria, prática e revisão.

INSTRUÇÃO
Monte um plano com um bloco por dia. Para cada bloco, entregue: objetivo, atividade prática e forma de verificação. Inclua um checkpoint em {{dia_do_checkpoint}} para revisar o bloco anterior e decidir o que manter ou ajustar no próximo. Separe "Fatos recebidos" de "Sugestões sujeitas à aprovação".

OBJETIVO
Terminar a semana com {{resultado_esperado}} e com um registro do que foi conferido.

FORMATO
Tabela com colunas: dia | horas | objetivo | atividade prática | verificação. Depois da tabela: checkpoint, lista "Depende da minha aprovação" e conferência final.

LIMITES
Não invente temas, prazos ou ferramentas que eu não informei. Use "a definir pelo estudante" quando faltar dado. Não envie mensagens, não crie eventos, não altere compromissos e não acesse contas externas sem minha aprovação.

Antes de executar, mostre como pretende fazer a tarefa e espere minha aprovação.
```

## O que fica fixo

- A ordem contexto → instrução → objetivo → formato → limites.
- A tabela com cinco colunas e a seção "Depende da minha aprovação".
- A separação entre fatos recebidos e sugestões.
- A regra de pedir o plano antes de executar e de não agir fora do plano.

## O que muda a cada uso

| Campo | Exemplo |
|---|---|
| `{{semana}}` | 23 a 29/11/2026 |
| `{{horas_totais}}` | 6 horas |
| `{{quantidade_blocos}}` | 3 |
| `{{dias_e_horarios}}` | segunda, quarta e sexta, 2h cada |
| `{{trilha_de_estudo}}` | IA aplicada no bootcamp |
| `{{dia_do_checkpoint}}` | quarta-feira |
| `{{resultado_esperado}}` | um bloco de prática revisado e anotado |

## Como foi testado

Na primeira tentativa a IA preencheu temas que eu não tinha informado. Ajustei acrescentando a regra "a definir pelo estudante" e o pedido de plano antes da execução. Com isso o resultado ficou verificável.
