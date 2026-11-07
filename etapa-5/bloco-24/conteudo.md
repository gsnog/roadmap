# Bloco 24: Código herdado e comunicação técnica

**Semana 24 · cerca de 5 horas**

## Objetivo

Entender e modificar com segurança um código que você não escreveu, e fazer perguntas técnicas por escrito que respeitem o tempo de quem responde.

## Como dividir a semana

- **2h de estudo:** os materiais abaixo, na ordem.
- **2h de prática:** os exercícios, **sem IA escrevendo código**. Se travar, use a IA só para explicar o conceito ou o erro.
- **1h de fechamento:** preencher o `resumo.md` e fazer a `avaliacao.md`.

Se não der tempo de terminar, continue na semana seguinte no mesmo ritmo. Nunca compense dobrando as horas.

## O que estudar (nesta ordem)

1. **Working Effectively with Legacy Code**, de Michael Feathers: as partes sobre testes de caracterização e sobre como encontrar pontos seguros para mudar.
2. Repositório **spring-petclinic** (github.com/spring-projects/spring-petclinic), uma aplicação Spring de exemplo para praticar a leitura.

## Prática

1. No spring-petclinic, siga um endpoint do curl até o banco com o debugger e desenhe o diagrama de sequência à mão.
2. Antes de alterar qualquer coisa, escreva um teste de caracterização que registre o comportamento atual. Depois faça uma pequena mudança via PR.
3. Escreva três perguntas "por quê" sobre decisões do código, no formato de mensagem assíncrona: contexto, o que você já tentou e a pergunta específica.
4. No trabalho: escolha com o seu mentor um serviço Java ou Spring que rode em dev, tenha logs legíveis e um dono acessível. Repita o exercício nele e leve as três perguntas ao dono. **Nada de código interno em IA.**

## Regra da semana

Nenhuma linha de código entra no projeto se você não conseguir explicá-la em voz alta.
