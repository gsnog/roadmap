# Bloco 12: Validação, tratamento de erros e logs na API

**Semana 12 · cerca de 5 horas**

## Objetivo

Fazer a API responder bem a entradas inválidas e erros, com mensagens claras, status corretos e logs úteis. Fechar a etapa com a primeira rodada de quebra intencional.

## Como dividir a semana

- **2h de estudo:** os materiais abaixo, na ordem.
- **2h de prática:** os exercícios, **sem IA escrevendo código**. Se travar, use a IA só para explicar o conceito ou o erro.
- **1h de fechamento:** preencher o `resumo.md` e fazer a `avaliacao.md`.

## O que estudar (nesta ordem)

1. Documentação do Spring sobre **Bean Validation** (`@Valid`, `@NotNull`, `@Positive`).
2. **Baeldung**: "Error Handling for REST with Spring" (`@ControllerAdvice`) e "Returning Errors Using ProblemDetail in Spring Boot".
3. RFC 9457, "Problem Details for HTTP APIs" (rfc-editor.org), o padrão de resposta de erro.
4. Documentação do **SLF4J** e do **Logback**, sobre níveis de log.

## Prática

1. Adicione validação a todos os endpoints e um handler global de erros que devolva respostas no formato ProblemDetail.
2. Adicione logs nos pontos importantes do fluxo, escolhendo o nível de cada um (DEBUG, INFO, WARN, ERROR) e justificando.
3. **Quebra intencional, sabendo o que quebrou** (veja modo-sabotagem.md): quebre de propósito três coisas no projeto (uma validação, uma regra de desconto, uma injeção de dependência) e anote o sintoma que cada uma produz. Essa é a sua coleção de assinaturas de erro.

## Regra da semana

Nenhuma linha de código entra no projeto se você não conseguir explicá-la em voz alta.
