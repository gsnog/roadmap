# Fase 1: Domínio em Java puro

**Acompanha a Etapa 1**

## Objetivo

Modelar o domínio sem nenhum framework, só com Java e testes simples.

## Entregas

- Classes `Produto`, `ItemPedido` e `Pedido`, com encapsulamento e validação no construtor.
- Duas promoções: desconto percentual e desconto por faixa de valor (por exemplo, 10% acima de R$ 100 e 15% acima de R$ 200).
- Exceções de domínio para pedido vazio, quantidade inválida e promoção inválida.
- Um `main` simples que cria pedidos e imprime o total com e sem desconto.
- Testes com JUnit desde o bloco 2.
- Repositório no GitHub com CI (GitHub Actions) rodando os testes a cada push e pull request, a partir do bloco 5.

## Restrições desta fase

- Sem Spring, sem banco, sem bibliotecas externas além do JUnit.
- Dinheiro em centavos ou `BigDecimal`.

## Critérios de aceite

- Você explica, linha por linha, qualquer classe do projeto.
- Existe pelo menos um teste para cada regra de desconto e para cada exceção.
- Há um ADR explicando como você modelou as promoções (herança ou interface) e por quê.
- O CI bloqueia um PR quando um teste falha.
