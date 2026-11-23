# Atalho: Resumo e Revisão de Aula

Use depois de assistir a uma aula ou ler um material, quando você precisa fixar o conteúdo sem transformar a IA na fonte da verdade. Adaptado de [Escrever e Melhorar Textos](01-escrever-e-melhorar-textos.md) e [Pesquisar um Assunto](03-pesquisar-um-assunto.md).

## Modelo

Copie o bloco, troque apenas o que está entre `{{ }}` e cole na IA que você usa.

```text
CONTEXTO
Estou estudando {{tema}} e tenho como fonte {{material_disponivel}}.

INSTRUÇÃO
Resuma o material e transforme-o em revisão. Separe:
1. Fatos que estão no material, com o trecho de origem;
2. Interpretações e exemplos criados por você;
3. Pontos que não foi possível confirmar no material;
4. Três perguntas de revisão e uma atividade prática curta.

OBJETIVO
Conseguir revisar {{tema}} em {{tempo_de_revisao}} e identificar o que ainda preciso pesquisar.

FORMATO
Tópicos curtos, até {{limite_de_linhas}} linhas, com as quatro seções acima e um título por seção.

LIMITES
Não invente conteúdo que não esteja no material. Se precisar de informação externa, diga o que verificou e apresente a fonte. Não escreva como se fosse eu: preserve minhas palavras quando eu fornecer um trecho. A decisão final sobre o que estudar é minha.
```

## O que fica fixo

- As quatro seções: fatos com origem, interpretações, incertezas e perguntas de revisão.
- A exigência de trecho de origem e de separar o que a IA criou.
- Os limites: não inventar, citar fonte externa quando houver e não falar por mim.

## O que muda a cada uso

| Campo | Exemplo |
|---|---|
| `{{tema}}` | prompts e delegação |
| `{{material_disponivel}}` | transcrição da aula 4 |
| `{{tempo_de_revisao}}` | 20 minutos |
| `{{limite_de_linhas}}` | 30 linhas |

## Como foi testado

Usei com um trecho curto de anotações. A primeira resposta misturava explicações da IA com o texto original; acrescentar "trecho de origem" e "interpretações criadas por você" resolveu a confusão. Ainda confiro o resumo contra o material antes de guardar.
