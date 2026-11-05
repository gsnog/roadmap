# Bloco 9: Redes e HTTP

**Semana 9 · cerca de 5 horas**

## Objetivo

Entender o caminho completo de uma requisição (DNS, TCP, TLS, HTTP) e dominar métodos, status codes e headers.

## Como dividir a semana

- **2h de estudo:** os materiais abaixo, na ordem.
- **2h de prática:** os exercícios, **sem IA escrevendo código**. Se travar, use a IA só para explicar o conceito ou o erro.
- **1h de fechamento:** preencher o `resumo.md` e fazer a `avaliacao.md`.

## O que estudar (nesta ordem)

1. **MDN Web Docs** (developer.mozilla.org), "Uma visão geral do HTTP", "Métodos de requisição HTTP" e "Códigos de status HTTP". Disponível em português.
2. Repositório **what-happens-when** no GitHub (alex/what-happens-when): o que acontece quando você digita um endereço no navegador.
3. Canal **Hussein Nasser** no YouTube, vídeos sobre HTTP e TCP.
4. Documentação do **curl** (curl.se), para fazer requisições pelo terminal.

## Prática

1. Faça requisições com `curl -v` para uma API pública e explique cada linha da saída: a resolução, o handshake, os headers enviados e recebidos.
2. Escreva um servidor HTTP mínimo em Java puro, sem Spring, usando `com.sun.net.httpserver.HttpServer`, que responda a um GET. Isso mostra o que o Spring faz por você.
3. Liste os endpoints que seu projeto vai ter na Fase 3 e decida o método e os status codes de cada um, justificando.

## Regra da semana

Nenhuma linha de código entra no projeto se você não conseguir explicá-la em voz alta.
