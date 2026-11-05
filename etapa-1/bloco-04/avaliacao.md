# Avaliação: Bloco 4, Exceções, lambdas, streams e leitura de stack trace

## Regras

- Responda **sem consultar material e sem IA**. Depois de responder, use o Prompt 4 do README para ser avaliada.
- **Resposta certa sem justificativa não passa.** Explique sempre o porquê.
- Nas perguntas com código, diga o resultado **antes** de executar. Depois execute e confira.
- Se não souber, escreva "não sei". Isso é informação útil, não fracasso.

## Perguntas

### 1.

Qual a diferença entre exceções checked e unchecked? Dê um exemplo de quando usar cada uma.

**Minha resposta:**



### 2.

Sem executar, diga o que este método retorna e explique por quê:

```java
int teste() {
    try {
        return 1;
    } finally {
        return 2;
    }
}
```

**Minha resposta:**



### 3.

Em um stack trace com "Caused by", qual parte normalmente aponta para a causa real do problema? Por quê?

**Minha resposta:**



### 4.

Por que capturar `Exception` genérico e não fazer nada (`catch (Exception e) {}`) é perigoso?

**Minha resposta:**



### 5.

Streams são preguiçosos (lazy). O que isso significa? Dê um exemplo de quando isso muda o comportamento do código.

**Minha resposta:**


## Critérios de aprovação

- Todas as respostas têm justificativa, e não só o resultado.
- Você usou pelo menos um exemplo do seu próprio projeto ou dos exercícios.
- Nenhuma resposta repete definição decorada sem explicar o mecanismo.
