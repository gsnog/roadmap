# Avaliação: Bloco 8, Threads e concorrência

## Regras

- Responda **sem consultar material e sem IA**. Depois de responder, use o Prompt 4 do README para ser avaliada.
- **Resposta certa sem justificativa não passa.** Explique sempre o porquê.
- Nas perguntas com código, diga o resultado **antes** de executar. Depois execute e confira.
- Se não souber, escreva "não sei". Isso é informação útil, não fracasso.

## Perguntas

### 1.

Duas threads incrementam o mesmo `int` 10.000 vezes cada. Por que o resultado costuma ser menor que 20.000? Explique o que acontece em `contador++`.

**Minha resposta:**



### 2.

Qual a diferença entre usar `synchronized` e `AtomicInteger` para resolver o problema acima? Quando cada um é mais adequado?

**Minha resposta:**



### 3.

O que é um deadlock? Quais são as condições para ele acontecer e como você o evitaria?

**Minha resposta:**



### 4.

Por que usar um `ExecutorService` em vez de criar `new Thread()` para cada tarefa?

**Minha resposta:**



### 5.

Qual a diferença entre `HashMap` e `ConcurrentHashMap` em um cenário com várias threads?

**Minha resposta:**


## Critérios de aprovação

- Todas as respostas têm justificativa, e não só o resultado.
- Você usou pelo menos um exemplo do seu próprio projeto ou dos exercícios.
- Nenhuma resposta repete definição decorada sem explicar o mecanismo.
