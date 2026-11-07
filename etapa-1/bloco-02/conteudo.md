# Bloco 2: Java: tipos, referências, orientação a objetos e primeiros testes

**Semana 2 · cerca de 5 horas**

## Objetivo

Entender a diferença entre primitivos e referências, como `==` e `equals` funcionam, quando usar herança, composição e interfaces, e escrever os primeiros testes com JUnit.

## Como dividir a semana

- **2h de estudo:** os materiais abaixo, na ordem.
- **2h de prática:** os exercícios, **sem IA escrevendo código**. Se travar, use a IA só para explicar o conceito ou o erro.
- **1h de fechamento:** preencher o `resumo.md` e fazer a `avaliacao.md`.

Se não der tempo de terminar, continue na semana seguinte no mesmo ritmo. Nunca compense dobrando as horas.

## O que estudar (nesta ordem)

1. **dev.java/learn** (tutorial oficial da Oracle): trilhas "Getting Started with Java" e "Classes and Objects".
2. **Use a Cabeça! Java** (Head First Java), capítulos sobre objetos, herança e polimorfismo. É didático e bom para construir intuição.
3. Canal **Loiane Groner** no YouTube, curso de Java básico, nas aulas sobre orientação a objetos, se você preferir vídeo em português.
4. **JUnit 5 User Guide** (junit.org/junit5): só as seções "Writing Tests" e "Assertions". O básico basta agora, porque a Fase 1 do projeto já exige testes. O aprofundamento vem no bloco 12.
5. Opcional, se sobrar tempo: **Effective Java**, Item 18 ("Favor composition over inheritance").

## Prática

1. Escreva, sem IA, as classes `Pedido`, `ItemPedido` e `Produto` em Java puro, com encapsulamento correto (atributos privados, validação no construtor).
2. Modele dois tipos de desconto (percentual e valor fixo) primeiro com herança e depois com uma interface. Anote as vantagens e desvantagens de cada versão.
3. Rode o código da pergunta 1 da avaliação e explique o resultado antes de executar.
4. Escreva testes JUnit para o construtor de `Pedido`: um caso válido e um caso que deve lançar exceção.

## Regra da semana

Nenhuma linha de código entra no projeto se você não conseguir explicá-la em voz alta.
