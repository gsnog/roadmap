# Bloco 14: Autenticação e autorização mínimas

**Semana 14 · cerca de 5 horas**

## Objetivo

Proteger a API com uma autenticação simples e regras de papel, entendendo onde isso acontece no caminho da requisição.

## Como dividir a semana

- **2h de estudo:** os materiais abaixo, na ordem.
- **2h de prática:** os exercícios, **sem IA escrevendo código**. Se travar, use a IA só para explicar o conceito ou o erro.
- **1h de fechamento:** preencher o `resumo.md` e fazer a `avaliacao.md`.

Se não der tempo de terminar, continue na semana seguinte no mesmo ritmo. Nunca compense dobrando as horas.

## O que estudar (nesta ordem)

1. **MDN Web Docs**: "Autenticação HTTP" (em português).
2. Documentação do **Spring Security**, seção "Architecture" do módulo Servlet, para entender a cadeia de filtros.
3. **OWASP API Security Top 10** (owasp.org): leia pelo menos os itens sobre autorização em nível de objeto e de função.

## Prática

1. Proteja os endpoints com uma API key, validada em um filtro.
2. Crie dois papéis, cliente e admin: só o admin cria promoções, e um cliente só vê os próprios pedidos.
3. Escreva testes que provem as respostas 401 e 403 nos casos certos.
4. Garanta que nenhuma chave fique em texto puro no código ou no repositório.

## Regra da semana

Nenhuma linha de código entra no projeto se você não conseguir explicá-la em voz alta.
