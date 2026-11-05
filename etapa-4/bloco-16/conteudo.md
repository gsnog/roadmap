# Bloco 16: Docker e ambiente de execução

**Semana 16 · cerca de 5 horas**

## Objetivo

Empacotar e rodar a aplicação com Docker, entender containers, volumes e redes, e diagnosticar problemas de configuração. Fechar a etapa com o Modo Sabotagem nível 1 e 2.

## Como dividir a semana

- **2h de estudo:** os materiais abaixo, na ordem.
- **2h de prática:** os exercícios, **sem IA escrevendo código**. Se travar, use a IA só para explicar o conceito ou o erro.
- **1h de fechamento:** preencher o `resumo.md` e fazer a `avaliacao.md`.

## O que estudar (nesta ordem)

1. Documentação oficial do Docker (docs.docker.com), seção "Get started".
2. Documentação do **Docker Compose**.
3. Aula "Command-line Environment" do **Missing Semester** (missing.csail.mit.edu), sobre processos, variáveis de ambiente e sinais.

## Prática

1. Escreva um Dockerfile para a aplicação (de preferência multi-stage) e um `docker-compose.yml` com a API e o PostgreSQL.
2. Configure a aplicação por variáveis de ambiente, sem nenhuma senha no código.
3. Faça a API falhar de propósito por configuração (porta errada, host do banco errado, variável ausente) e anote o sintoma de cada falha.
4. **Modo Sabotagem, níveis 1 e 2** (veja modo-sabotagem.md): primeira rodada às cegas.

## Regra da semana

Nenhuma linha de código entra no projeto se você não conseguir explicá-la em voz alta.
