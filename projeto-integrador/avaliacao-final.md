# Avaliação final: defesa

Esta avaliação não é sobre escrever mais código. É sobre **sustentar** o que você construiu. **Faça com uma pessoa, de preferência o seu mentor.** O prompt no final serve para treinar antes, não para substituir a defesa com uma pessoa.

## Parte 1: defesa das decisões (cerca de 30 min)

Explique, sem consultar o código:

1. Como uma requisição de criação de pedido percorre o sistema, do curl até o banco e de volta.
2. Como você modelou as promoções e a regra de combinação. Que alternativa você descartou e por quê?
3. Por que você escolheu lock otimista ou pessimista para o estoque? Em que cenário você mudaria de ideia?
4. Como o snapshot garante que um pedido antigo seja reproduzível?
5. Por que dinheiro em centavos ou `BigDecimal`, e não `double`?
6. Quais índices você criou e que evidência mostrou que eles ajudam?
7. Como você garante que um retry não cria um pedido duplicado?
8. Como você fez a migração de schema sem perder dados e sem indisponibilidade?

## Parte 2: cenário sob pressão (cerca de 30 min)

O avaliador escolhe um destes cenários, ou cria outro. Você tem 30 minutos para diagnosticar e propor a correção, explicando o raciocínio em voz alta.

- "Desde a última versão, alguns clientes estão recebendo um desconto maior que o permitido."
- "A criação de pedidos ficou lenta no horário de pico, mas a CPU da aplicação está baixa."
- "Durante uma promoção, o estoque de um produto ficou negativo."

## Parte 3: autoavaliação honesta

Responda por escrito:

1. O que eu hoje consigo fazer sozinha que não conseguia no início?
2. Em que ponto eu ainda dependeria de ajuda? De que tipo?
3. Qual foi o erro mais difícil que eu diagnostiquei e o que ele me ensinou?
4. O que eu estudaria a seguir? (Spoiler: System Design.)

## Critérios

- As decisões são defendidas com trade-offs, e não com "porque é o padrão".
- No cenário sob pressão, o raciocínio segue sintoma, hipóteses, evidências e causa, em vez de tentativa e erro.
- A autoavaliação reconhece limites concretos.

## Prompt para treinar a defesa com a IA

```
Quero fazer a avaliação final de defesa do meu projeto integrador
(API de Pedidos com Promoções, Java + Spring Boot + PostgreSQL + Docker).

Seja um avaliador técnico rigoroso. Faça as perguntas da Parte 1 uma por vez,
aprofunde com perguntas de acompanhamento quando minha resposta for vaga e
não aceite respostas sem trade-offs. Depois conduza um cenário da Parte 2,
me dando informações só quando eu pedir evidências específicas.
No final, me dê um parecer honesto sobre o que está sólido e o que ainda está raso.
```
