# Fase 5: Observabilidade, sabotagem e defesa

**Acompanha a Etapa 5**

## Objetivo

Tornar o sistema observável, diagnosticar falhas às cegas e preparar a defesa final.

## Entregas

- **Primeiro, na transição da Fase 4 para a 5:** uma migração de schema com dados existentes, no padrão expand e contract, sem perder dados e com a versão antiga e a nova da aplicação funcionando durante a transição (bloco 23).
- Actuator com health check e métricas.
- Logs em JSON com ID de correlação por requisição.
- Uma métrica de negócio, como a quantidade de pedidos com desconto.
- Relatórios de incidente das rodadas de sabotagem dos blocos 25 e 26 (a do 26 conduzida por uma pessoa).
- Pasta `docs/adr/` completa com as decisões do projeto.

## Restrições desta fase

- Todo erro em produção simulada precisa ser rastreável pelos logs a partir do ID de correlação.

## Critérios de aceite

- Uma consulta prova que nenhum dado se perdeu na migração.
- Você encontra a causa de um erro só pelos logs e métricas, sem abrir o código primeiro.
- Os relatórios de incidente têm evidências que sustentam a causa raiz.
- Você está pronta para a avaliação final.
