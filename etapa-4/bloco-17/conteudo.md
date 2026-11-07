# Bloco 17: Índices e performance de consultas

**Semana 17 · cerca de 5 horas**

## Objetivo

Entender como um índice funciona, ler um plano de execução e saber por que uma consulta está lenta.

## Como dividir a semana

- **2h de estudo:** os materiais abaixo, na ordem.
- **2h de prática:** os exercícios, **sem IA escrevendo código**. Se travar, use a IA só para explicar o conceito ou o erro.
- **1h de fechamento:** preencher o `resumo.md` e fazer a `avaliacao.md`.

Se não der tempo de terminar, continue na semana seguinte no mesmo ritmo. Nunca compense dobrando as horas.

## O que estudar (nesta ordem)

1. **Use The Index, Luke!** (use-the-index-luke.com): capítulos sobre a anatomia de um índice e a cláusula WHERE. Gratuito.
2. Documentação do PostgreSQL: "Using EXPLAIN" e "Indexes".
3. Retome o que você estudou sobre árvores no bloco 7.

## Prática

1. Insira pelo menos 1 milhão de linhas em uma tabela de pedidos (com `generate_series`) e meça uma consulta com `EXPLAIN ANALYZE` antes e depois de criar um índice.
2. Crie um índice composto e teste consultas que o usam e que não o usam, mudando a ordem das colunas no filtro.
3. Escreva uma consulta que não use o índice mesmo ele existindo (por exemplo, aplicando uma função na coluna) e explique por quê.

## Regra da semana

Nenhuma linha de código entra no projeto se você não conseguir explicá-la em voz alta.
