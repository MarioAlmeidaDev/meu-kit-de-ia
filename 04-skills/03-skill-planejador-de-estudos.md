# Skill: Planejador de Estudos

Skill criada a partir do [Planejador Semanal de Estudos](../01-prompts/06-planejador-semanal-de-estudos.md), o atalho que mais usei. Ela transforma o atalho numa forma de trabalhar, seguindo o [guia de estrutura](01-como-estruturar-uma-skill.md).

```text
OBJETIVO
Organizar uma semana de estudos e tarefas em blocos compatíveis com o tempo realmente disponível, entregando um plano que pode ser conferido antes de qualquer ação.

INSTRUÇÕES
- Trate apenas as informações recebidas como fatos.
- Marque todo o resto como sugestão sujeita à aprovação.
- Quando faltar informação, escreva "a definir pelo estudante" em vez de presumir.
- Não tome decisões por mim; apresente opções ou campos em aberto.
- Não envie mensagens, não crie eventos, não altere compromissos e não acesse contas externas sem autorização explícita.
- Mostre o plano de trabalho antes de produzir o plano final.

PROCEDIMENTO
1. Listar os fatos recebidos: período, horas, blocos, trilha e checkpoint.
2. Separar explicitamente fatos de sugestões.
3. Distribuir as horas nos blocos informados, sem ultrapassar o total.
4. Definir para cada bloco: objetivo, atividade prática e verificação.
5. Preparar o checkpoint para revisar o bloco anterior e decidir o que manter ou ajustar.
6. Listar o que depende da minha aprovação.
7. Conferir o plano antes de entregá-lo.

VERIFICAÇÕES
- A soma das horas é igual ao total informado.
- Os blocos estão nas datas informadas.
- Todos os blocos têm objetivo, prática e verificação.
- O checkpoint está no dia combinado e não gera ação externa.
- Fatos e sugestões estão em seções separadas.
- Nenhum dado foi inventado e nenhuma ação externa foi executada.

EXCEÇÕES
- Se o tempo disponível não couber nos blocos, pare e pergunte antes de remover conteúdo.
- Se o tema do bootcamp não tiver sido informado, mantenha o campo como "a definir pelo estudante".
- Se houver ambiguidade no checkpoint, apresente duas opções e deixe a escolha comigo.

FORMATO DE SAÍDA
Fatos recebidos
Sugestões sujeitas à aprovação
Tabela: dia | horas | objetivo | atividade prática | verificação
Checkpoint
Depende da minha aprovação
Conferência executada
```
