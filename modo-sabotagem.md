# Modo Sabotagem

O objetivo é treinar o músculo de **diagnosticar um problema que você não sabe qual é**, o que é bem diferente de consertar um bug que você mesma escreveu.

## Regra de ouro

Primeiro você quebra **sabendo** o que quebrou, para aprender a assinatura de cada sintoma. Só depois vem a sabotagem às cegas.

## Quando rodar

| Momento | Tipo | Nível |
|---|---|---|
| Bloco 12 (fim da etapa 3) | Quebra intencional, sabendo o que quebrou | Lógica e código |
| Bloco 16 (fim da etapa 4) | Às cegas | 1 (lógica) e 2 (configuração) |
| Bloco 18 | Às cegas, com relatório completo | 1 e 2 |
| Bloco 19 | Às cegas | 3 (infraestrutura: banco, Docker, rede, recursos) |

## Níveis

- **Nível 1, lógica e código:** uma regra de desconto errada, um `equals` quebrado, uma condição de corrida, uma exceção engolida.
- **Nível 2, configuração:** uma variável de ambiente errada, um pool de conexões pequeno demais, um timeout mal configurado, um bean com escopo errado.
- **Nível 3, infraestrutura:** banco fora do ar, índice removido, container sem memória suficiente, rede entre containers quebrada.

## Prompt 3: rodar a sabotagem

```
Quero rodar uma sessão de Modo Sabotagem no meu projeto.

Regras:
1. Meu projeto está funcionando e commitado. Crie uma branch separada e
   injete de 1 a 3 falhas realistas de nível [1 = lógica/código |
   2 = configuração | 3 = infraestrutura].
2. NÃO me diga o que você fez.
3. Me entregue apenas o SINTOMA, como se fosse um alerta real
   (ex: "usuários relatando erro no fluxo X desde as 14h").
4. Escolha falhas que acontecem de verdade e produzem sintomas
   observáveis — nada de pegadinha esotérica.

Eu vou diagnosticar sozinha, com timebox de 30–45 min. Não vou olhar o
diff até fechar o diagnóstico e escrever meu relatório de incidente:
sintoma → hipóteses (inclusive as descartadas) → evidências → causa raiz →
correção → prevenção.

Se eu travar, me dê dicas em estágios, uma de cada vez:
  1ª dica: em qual camada está o problema
  2ª dica: qual ferramenta revelaria a evidência
  3ª dica: qual componente olhar

Depois que eu entregar o relatório, revise como um post-mortem: as
evidências que eu levantei sustentam a causa raiz? Achar por sorte não conta.
```

Como a IA não tem acesso direto ao seu repositório em uma conversa comum, uma forma prática é pedir que ela gere o patch da sabotagem, aplicar com `git apply` sem ler o conteúdo, e só abrir o diff depois do relatório. Outra opção é pedir a um colega para sabotar o projeto.

## Modelo de relatório de incidente

```
# Incidente: [título]

**Data:** · **Tempo até o diagnóstico:**

## Sintoma
## Hipóteses (incluindo as descartadas e por que foram descartadas)
## Evidências (logs, métricas, dumps, consultas)
## Causa raiz
## Correção
## Prevenção (teste, alerta ou validação que teria evitado ou detectado antes)
## O que eu faria diferente no diagnóstico
```
