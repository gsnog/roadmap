# Bloco 4: Exceções, lambdas, streams e leitura de stack trace

**Semana 4 · cerca de 5 horas**

## Objetivo

Tratar erros de forma consciente, usar streams e lambdas sabendo o que acontece por baixo, e ler qualquer stack trace até encontrar a causa.

## Como dividir a semana

- **2h de estudo:** os materiais abaixo, na ordem.
- **2h de prática:** os exercícios, **sem IA escrevendo código**. Se travar, use a IA só para explicar o conceito ou o erro.
- **1h de fechamento:** preencher o `resumo.md` e fazer a `avaliacao.md`.

## O que estudar (nesta ordem)

1. **dev.java/learn**, trilhas "Exceptions" e "Lambda Expressions" e "The Stream API".
2. **Baeldung**: "Checked and Unchecked Exceptions in Java" e "The Java 8 Stream API Tutorial".
3. **Effective Java**, Itens 69 a 77 (capítulo sobre exceções). Leia pelo menos os itens 69, 70 e 73.

## Prática

1. Crie exceções de domínio para o seu projeto (por exemplo `PedidoVazioException`) e decida, justificando, se cada uma deve ser checked ou unchecked.
2. Reescreva três loops do seu projeto usando streams, e depois o contrário. Compare a legibilidade.
3. Provoque de propósito um `NullPointerException`, um `ClassCastException` e um `ConcurrentModificationException`. Para cada um, leia o stack trace e marque a linha da causa.

## Regra da semana

Nenhuma linha de código entra no projeto se você não conseguir explicá-la em voz alta.
