# Fase 2: Estruturas certas e concorrência

**Acompanha a Etapa 2**

## Objetivo

Escolher as estruturas de dados conscientemente e tornar o estoque seguro sob concorrência.

## Entregas

- Catálogo de produtos indexado por ID, com a estrutura escolhida justificada pela complexidade das operações.
- Cashback progressivo como terceira promoção, com regra de combinação entre as três.
- Um serviço de estoque em memória usado por várias threads ao mesmo tempo.
- Um teste que dispara 100 compras simultâneas do mesmo produto com estoque 10.

## Restrições desta fase

- O estoque nunca pode ficar negativo.
- O cálculo precisa ser determinístico: a ordem de aplicação das promoções é fixa e documentada.

## Critérios de aceite

- O teste de concorrência passa em 20 execuções seguidas.
- Você mostra a versão com condição de corrida e explica por que ela falha.
- Há um ADR sobre a regra de combinação das promoções.
