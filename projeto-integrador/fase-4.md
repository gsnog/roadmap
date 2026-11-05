# Fase 4: PostgreSQL, transações e Docker

**Acompanha a Etapa 4**

## Objetivo

Persistir os dados com consistência e rodar tudo em containers.

## Entregas

- Modelagem das tabelas com constraints e migrações (Flyway ou Liquibase).
- Snapshot das promoções aplicadas gravado junto com o pedido, com a regra e o valor de cada desconto.
- Controle de estoque com lock otimista ou pessimista, com a escolha justificada.
- Índices para as consultas mais usadas, validados com `EXPLAIN ANALYZE`.
- Dockerfile e `docker-compose.yml` com a API e o PostgreSQL, configurados por variáveis de ambiente.

## Restrições desta fase

- Nenhuma senha no código.
- Consultar um pedido antigo mostra exatamente as promoções aplicadas na época, mesmo que as regras tenham mudado.

## Critérios de aceite

- `docker compose up` sobe tudo do zero em uma máquina limpa.
- O teste de compras simultâneas passa contra o banco real.
- Não existe problema N+1 na listagem de pedidos.
- Você completou a primeira rodada de sabotagem com relatório de incidente.
