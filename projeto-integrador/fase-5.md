# Fase 5: Observabilidade, sabotagem e defesa

**Acompanha a Etapa 5**

## Objetivo

Tornar o sistema observável, diagnosticar falhas às cegas e preparar a defesa final.

## Entregas

- Actuator com health check e métricas.
- Logs em JSON com ID de correlação por requisição.
- Uma métrica de negócio, como a quantidade de pedidos com desconto.
- Relatórios de incidente das rodadas de sabotagem dos blocos 18 e 19.
- Pasta `docs/adr/` completa com as decisões do projeto.

## Restrições desta fase

- Todo erro em produção simulada precisa ser rastreável pelos logs a partir do ID de correlação.

## Critérios de aceite

- Você encontra a causa de um erro só pelos logs e métricas, sem abrir o código primeiro.
- Os relatórios de incidente têm evidências que sustentam a causa raiz.
- Você está pronta para a avaliação final.
