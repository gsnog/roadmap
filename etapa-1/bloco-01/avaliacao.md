# Avaliação: Bloco 1, Ferramentas: Git, terminal e debugger

## Regras

- Responda **sem consultar material e sem IA**. Depois de responder, use o Prompt 4 do README para ser avaliada.
- **Resposta certa sem justificativa não passa.** Explique sempre o porquê.
- Nas perguntas com código, diga o resultado **antes** de executar. Depois execute e confira.
- Se não souber, escreva "não sei". Isso é informação útil, não fracasso.

## Perguntas

### 1.

O que acontece, no nível dos objetos do Git, quando você faz um commit? Por que o Git consegue voltar a qualquer versão?

**Minha resposta:**
quando eu faço um commit o git cria um snapshot do codigo naquele momento e ele consegue voltar a qualquer versao pq esses snapshots formam um historico e sao ligados pelos commit entao ele consegue refazer o caminho de volta.


### 2.

No debugger, qual a diferença entre step over e step into? Dê um exemplo em que usar o errado faria você perder a causa de um bug.

**Minha resposta:**
o step over vai para a proxima linha e o step into entra dentro do metodo que esta sendo chamado. usar o errado me faria perder o bug pq talvez o bug estivesse dentro da logica do metodo e eu pulei direto para a proxima linha.


### 3.

Explique o que estes comandos fazem e por que funcionam juntos: `cat app.log | grep ERROR | wc -l`.

**Minha resposta:**
o cat le o arquivo o grep filtra e o wc conta quantos tem. eles funcionam juntos por conta da barra que funciona como um cano de conexão.

## Critérios de aprovação

- Todas as respostas têm justificativa, e não só o resultado.
- Você usou pelo menos um exemplo do seu próprio projeto ou dos exercícios.
- Nenhuma resposta repete definição decorada sem explicar o mecanismo.
