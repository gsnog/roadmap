# Fase 3: API REST com Spring Boot

**Acompanha a Etapa 3**

## Objetivo

Expor o domínio como uma API e garantir o comportamento com testes.

## Entregas

- Endpoints para criar pedido, consultar pedido e listar promoções, com métodos e status codes justificados.
- Validação de entrada e tratamento global de erros com ProblemDetail.
- Testes unitários do domínio e testes de integração dos endpoints com MockMvc.
- Logs nos pontos importantes do fluxo, com níveis justificados.
- Autenticação por API key e dois papéis: cliente e admin. Só o admin cria promoções, e um cliente só vê os próprios pedidos.

## Restrições desta fase

- Os dados ainda ficam em memória.
- Nenhum stack trace é devolvido ao cliente.

## Critérios de aceite

- Você explica o caminho de uma requisição do curl até o seu controller.
- Toda regra de negócio tem pelo menos um teste que falha se você quebrá-la.
- Você registrou as assinaturas de erro da quebra intencional do bloco 13.
- Existem testes que provam as respostas 401 e 403.
