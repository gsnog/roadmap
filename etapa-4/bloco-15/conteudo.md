# Bloco 15: Transações, isolamento e concorrência no banco

**Semana 15 · cerca de 5 horas**

## Objetivo

Entender ACID, níveis de isolamento, locks otimista e pessimista, e as armadilhas do `@Transactional` e do JPA.

## Como dividir a semana

- **2h de estudo:** os materiais abaixo, na ordem.
- **2h de prática:** os exercícios, **sem IA escrevendo código**. Se travar, use a IA só para explicar o conceito ou o erro.
- **1h de fechamento:** preencher o `resumo.md` e fazer a `avaliacao.md`.

## O que estudar (nesta ordem)

1. Documentação do PostgreSQL: "Transaction Isolation" e "Explicit Locking".
2. **Designing Data-Intensive Applications**, de Martin Kleppmann, capítulo 7 ("Transactions"). Este é o primeiro contato com o livro que você vai usar no System Design.
3. Blog de **Vlad Mihalcea** (vladmihalcea.com): artigos sobre o problema N+1 e sobre optimistic locking com JPA.
4. **Baeldung**: "Transactions with Spring and JPA".

## Prática

1. Persista o projeto no PostgreSQL com Spring Data JPA.
2. Simule duas compras simultâneas do último item em estoque. Mostre o problema e corrija primeiro com lock otimista (`@Version`) e depois com lock pessimista. Compare os dois.
3. Provoque o problema N+1 ao listar pedidos com itens, veja as consultas no log e corrija.
4. Chame um método `@Transactional` de dentro da mesma classe e observe que a transação não é aplicada. Explique por quê.

## Regra da semana

Nenhuma linha de código entra no projeto se você não conseguir explicá-la em voz alta.
