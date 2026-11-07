# Bloco 8: Memória da JVM e garbage collector

**Semana 8 · cerca de 5 horas**

## Objetivo

Entender onde os objetos vivem (stack e heap), como o garbage collector funciona e como diagnosticar problemas de memória.

## Como dividir a semana

- **2h de estudo:** os materiais abaixo, na ordem.
- **2h de prática:** os exercícios, **sem IA escrevendo código**. Se travar, use a IA só para explicar o conceito ou o erro.
- **1h de fechamento:** preencher o `resumo.md` e fazer a `avaliacao.md`.

Se não der tempo de terminar, continue na semana seguinte no mesmo ritmo. Nunca compense dobrando as horas.

## O que estudar (nesta ordem)

1. **Baeldung**: "Stack Memory and Heap Space in Java" e "JVM Garbage Collectors".
2. Documentação da Oracle: "HotSpot Virtual Machine Garbage Collection Tuning Guide". **Leia só por cima**, para saber que os coletores existem e o que os diferencia. Tuning não é o objetivo aqui.
3. **VisualVM** (visualvm.github.io): ferramenta gratuita para observar memória e threads de uma aplicação em execução.
4. Documentação do comando `jcmd`, para gerar heap dump e informações da JVM.

## Prática

1. Escreva um programa que vaze memória de propósito (por exemplo, adicionando objetos em uma lista estática para sempre). Observe a memória subindo no VisualVM até o `OutOfMemoryError`.
2. Gere um `StackOverflowError` com uma recursão sem fim e leia o stack trace.
3. Rode o mesmo programa com `-Xmx` diferentes e observe a mudança de comportamento.
4. Pesquise o que mudou na memória entre Java 11 e versões recentes (por exemplo, os compact object headers do Java 25) e relacione com a migração que você fez no trabalho.

## Regra da semana

Nenhuma linha de código entra no projeto se você não conseguir explicá-la em voz alta.
