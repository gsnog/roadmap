# Bloco 3: Coleções e generics

**Semana 3 · cerca de 5 horas**

## Objetivo

Saber escolher a coleção certa para cada problema, entender como o HashMap funciona por dentro e por que o contrato entre equals e hashCode importa.

## Como dividir a semana

- **2h de estudo:** os materiais abaixo, na ordem.
- **2h de prática:** os exercícios, **sem IA escrevendo código**. Se travar, use a IA só para explicar o conceito ou o erro.
- **1h de fechamento:** preencher o `resumo.md` e fazer a `avaliacao.md`.

Se não der tempo de terminar, continue na semana seguinte no mesmo ritmo. Nunca compense dobrando as horas.

## O que estudar (nesta ordem)

1. **dev.java/learn**, trilha "The Collections Framework".
2. **Baeldung** (baeldung.com): artigos "A Guide to Java HashMap" e "Guide to hashCode() in Java".
3. **Effective Java**, Itens 10 e 11, sobre o contrato de equals e hashCode.
4. dev.java/learn, trilha "Generics".

## Prática

1. Adicione ao seu `Pedido` uma lista de itens e um mapa de produtos por ID. Justifique por escrito cada escolha de coleção.
2. Crie uma classe `Produto` sem `hashCode`, coloque dois produtos "iguais" em um `HashSet` e observe o tamanho do conjunto. Depois implemente `equals` e `hashCode` corretamente e compare.
3. Escreva um método genérico `<T> T maisFrequente(List<T> lista)` sem IA.

## Regra da semana

Nenhuma linha de código entra no projeto se você não conseguir explicá-la em voz alta.
