# Bloco 22: Observabilidade básica

**Semana 22 · cerca de 5 horas**

## Objetivo

Tornar a aplicação observável: logs estruturados, métricas e health checks, e entender o que cada um responde.

## Como dividir a semana

- **2h de estudo:** os materiais abaixo, na ordem.
- **2h de prática:** os exercícios, **sem IA escrevendo código**. Se travar, use a IA só para explicar o conceito ou o erro.
- **1h de fechamento:** preencher o `resumo.md` e fazer a `avaliacao.md`.

Se não der tempo de terminar, continue na semana seguinte no mesmo ritmo. Nunca compense dobrando as horas.

## O que estudar (nesta ordem)

1. Documentação do **Spring Boot Actuator** e do **Micrometer**.
2. Projeto **logstash-logback-encoder** no GitHub, para gerar logs em JSON.
3. **Site Reliability Engineering**, livro do Google (sre.google/books, gratuito), capítulo 6, "Monitoring Distributed Systems". Leia com atenção a parte sobre os quatro sinais de ouro.

## Prática

1. Adicione o Actuator ao projeto e exponha health check e métricas.
2. Transforme os logs em JSON e adicione um ID de correlação por requisição (via MDC), que aparece em todos os logs daquela requisição.
3. Crie uma métrica de negócio (por exemplo, quantidade de pedidos com desconto) e observe-a mudando enquanto você faz requisições.

## Regra da semana

Nenhuma linha de código entra no projeto se você não conseguir explicá-la em voz alta.
