# Bloco 23: Migração de schema com dado vivo

**Semana 23 · cerca de 5 horas**

## Objetivo

Mudar o modelo do banco com a aplicação rodando e dados existentes, sem perder dados e sem indisponibilidade.

## Como dividir a semana

- **2h de estudo:** os materiais abaixo, na ordem.
- **2h de prática:** os exercícios, **sem IA escrevendo código**. Se travar, use a IA só para explicar o conceito ou o erro.
- **1h de fechamento:** preencher o `resumo.md` e fazer a `avaliacao.md`.

Se não der tempo de terminar, continue na semana seguinte no mesmo ritmo. Nunca compense dobrando as horas.

## O que estudar (nesta ordem)

1. **Martin Fowler** (martinfowler.com): "Parallel Change", sobre o padrão expand e contract, e "Evolutionary Database Design".
2. Documentação do **Flyway**, sobre migrações versionadas.

## Prática

1. Faça uma mudança de schema com dados já existentes (por exemplo, renomear uma coluna ou mover os descontos aplicados para uma tabela própria) usando expand, migrar e contract.
2. Escreva um backfill em lotes para os dados antigos.
3. Durante a transição, confirme que a versão antiga e a versão nova da aplicação funcionam ao mesmo tempo.
4. Escreva uma consulta que prove que nenhum dado se perdeu.

## Regra da semana

Nenhuma linha de código entra no projeto se você não conseguir explicá-la em voz alta.
