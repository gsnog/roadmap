# Bloco 19: Idempotência e retries

**Semana 19 · cerca de 5 horas**

## Objetivo

Garantir que uma requisição repetida, por timeout ou retry, nunca crie um pedido duplicado.

## Como dividir a semana

- **2h de estudo:** os materiais abaixo, na ordem.
- **2h de prática:** os exercícios, **sem IA escrevendo código**. Se travar, use a IA só para explicar o conceito ou o erro.
- **1h de fechamento:** preencher o `resumo.md` e fazer a `avaliacao.md`.

Se não der tempo de terminar, continue na semana seguinte no mesmo ritmo. Nunca compense dobrando as horas.

## O que estudar (nesta ordem)

1. Blog da **Stripe**: "Designing robust and predictable APIs with idempotency" (stripe.com/blog/idempotency).
2. Documentação da API da Stripe, seção "Idempotent requests", como exemplo de implementação real.
3. **Amazon Builders' Library** (aws.amazon.com/builders-library): "Making retries safe with idempotent APIs" e "Timeouts, retries, and backoff with jitter".

## Prática

1. Implemente o header `Idempotency-Key` no endpoint de criação de pedido, guardando a chave com uma constraint única no banco.
2. Teste: a mesma chave enviada duas vezes devolve o mesmo pedido, e a mesma chave com um corpo diferente devolve erro.
3. Dispare duas requisições simultâneas com a mesma chave e confirme que só um pedido é criado. Relacione com o bloco 18.
4. Simule um timeout no cliente seguido de retry e confirme que nada é duplicado.

## Regra da semana

Nenhuma linha de código entra no projeto se você não conseguir explicá-la em voz alta.
