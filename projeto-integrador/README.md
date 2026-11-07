# Projeto integrador: API de Pedidos com Promoções

Um sistema de pedidos com cálculo de promoções, construído do zero ao longo das 5 etapas. Segundo o mentor, ele se parece com problemas reais. O tema é parecido com o da sua entrevista, de propósito: no fim, você vai conseguir defender com experiência própria as respostas que antes dependiam da IA.

## Regras gerais

- **Sem IA escrevendo código.** A IA só explica conceitos e erros.
- **Tudo versionado no Git,** com commits pequenos e mensagens que expliquem o porquê. A partir do bloco 5, **toda mudança entra por pull request**, com descrição e CI passando.
- **Toda decisão importante é registrada** em um ADR curto na pasta `docs/adr/` do projeto: contexto, opções consideradas, decisão e consequências.
- **Cada fase só termina quando os critérios de aceite passam.**

## Restrições (valem para todas as fases)

- **Dinheiro em centavos (`long`) ou `BigDecimal`,** nunca `double`. Você precisa saber explicar por quê.
- **Um pedido pode ter várias promoções ao mesmo tempo,** com uma regra de combinação clara: o que acumula, o que é exclusivo e a ordem de aplicação.
- **O desconto total de um pedido nunca pode passar de 50% do valor,** e o total nunca pode ser negativo.
- **O estoque nunca pode ficar negativo,** mesmo com várias compras simultâneas.
- **O cálculo de um pedido precisa ser reproduzível:** dado o mesmo pedido e as mesmas regras, o resultado é sempre o mesmo.
- **A partir da Fase 4, um retry nunca cria um pedido duplicado.**

## Fases

| Fase | Etapa | O que muda |
|---|---|---|
| [1](fase-1.md) | 1 | Domínio em Java puro, sem framework |
| [2](fase-2.md) | 2 | Estruturas certas e concorrência no estoque |
| [3](fase-3.md) | 3 | API REST com Spring Boot, testes e autenticação |
| [4](fase-4.md) | 4 | PostgreSQL, transações, idempotência e Docker |
| [5](fase-5.md) | 5 | Migração com dado vivo, observabilidade, sabotagem e defesa |
