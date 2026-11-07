# Bloco 11: Spring Boot por dentro

**Semana 11 · cerca de 5 horas**

## Objetivo

Entender o que o Spring faz por baixo: inversão de controle, injeção de dependência, auto-configuração e o caminho de uma requisição até o seu controller.

## Como dividir a semana

- **2h de estudo:** os materiais abaixo, na ordem.
- **2h de prática:** os exercícios, **sem IA escrevendo código**. Se travar, use a IA só para explicar o conceito ou o erro.
- **1h de fechamento:** preencher o `resumo.md` e fazer a `avaliacao.md`.

Se não der tempo de terminar, continue na semana seguinte no mesmo ritmo. Nunca compense dobrando as horas.

## O que estudar (nesta ordem)

1. **spring.io/guides**: "Building a RESTful Web Service" e "Building an Application with Spring Boot".
2. Documentação do Spring Framework, seção "The IoC Container".
3. Canal **Michelli Brito** no YouTube, vídeos de Spring Boot em português.
4. **Baeldung**: "Intro to Inversion of Control and Dependency Injection with Spring" e "An Intro to the Spring DispatcherServlet".

## Prática

1. Transforme o projeto em uma API Spring Boot com camadas controller, service e repository (ainda com dados em memória).
2. Coloque um breakpoint no seu controller e, pelo stack trace no debugger, identifique as classes do Spring por onde a requisição passou antes de chegar ao seu código.
3. Rode a aplicação com `--debug` e leia o relatório de auto-configuração. Escolha três itens e explique o que cada um configurou.

## Regra da semana

Nenhuma linha de código entra no projeto se você não conseguir explicá-la em voz alta.
