# Bloco 9: Threads e concorrência

**Semana 9 · cerca de 5 horas**

## Objetivo

Entender o que é uma thread, por que condições de corrida acontecem e como evitá-las com as ferramentas do Java.

## Como dividir a semana

- **2h de estudo:** os materiais abaixo, na ordem.
- **2h de prática:** os exercícios, **sem IA escrevendo código**. Se travar, use a IA só para explicar o conceito ou o erro.
- **1h de fechamento:** preencher o `resumo.md` e fazer a `avaliacao.md`.

Se não der tempo de terminar, continue na semana seguinte no mesmo ritmo. Nunca compense dobrando as horas.

## O que estudar (nesta ordem)

1. **dev.java/learn**, trilha "Concurrency".
2. **Java Concurrency in Practice**, de Brian Goetz, **só os capítulos 1 e 2**.
3. **Baeldung**: "A Guide to the Java ExecutorService" e "Guide to java.util.concurrent.atomic".
4. JEP 444 (openjdk.org), sobre virtual threads, para ter uma noção do que mudou nas versões recentes.

## Prática

1. Crie um contador compartilhado por duas threads, cada uma incrementando 10.000 vezes. Rode várias vezes e anote os resultados. Depois corrija com `synchronized` e com `AtomicInteger`.
2. Simule o estoque do seu projeto sendo reduzido por várias threads ao mesmo tempo, provoque estoque negativo e corrija.
3. Crie um deadlock de propósito com duas threads e dois locks. Gere um thread dump com `jcmd <pid> Thread.print` e encontre o deadlock nele.

## Regra da semana

Nenhuma linha de código entra no projeto se você não conseguir explicá-la em voz alta.
