# Bloco 18: Diagnóstico de incidentes

**Semana 18 · cerca de 5 horas**

## Objetivo

Aplicar um método de diagnóstico em problemas que você não causou: levantar hipóteses, buscar evidências e chegar à causa raiz.

## Como dividir a semana

- **2h de estudo:** os materiais abaixo, na ordem.
- **2h de prática:** os exercícios, **sem IA escrevendo código**. Se travar, use a IA só para explicar o conceito ou o erro.
- **1h de fechamento:** preencher o `resumo.md` e fazer a `avaliacao.md`.

## O que estudar (nesta ordem)

1. **Site Reliability Engineering**, capítulo 12 ("Effective Troubleshooting") e capítulo 15 ("Postmortem Culture").
2. Documentação do `jcmd` e do `jstack`, para thread dumps.
3. **Eclipse Memory Analyzer (MAT)**, para analisar heap dumps.

## Prática

1. Gere um heap dump do programa com vazamento do bloco 7 e encontre, no Eclipse MAT, o objeto que está acumulando memória.
2. Gere um thread dump da aplicação sob carga e identifique o que cada thread está fazendo.
3. **Modo Sabotagem às cegas, níveis 1 e 2** (veja modo-sabotagem.md), com relatório de incidente completo.

## Regra da semana

Nenhuma linha de código entra no projeto se você não conseguir explicá-la em voz alta.
