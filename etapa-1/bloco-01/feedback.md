# Feedback: Bloco 1, Ferramentas: Git, terminal e debugger

> Preenchido depois da correção (Prompt 4 do README).

**Data da avaliação:** 2026-11-12

**Resultado:** ☐ Aprovado · ☒ Revisar antes de avançar

Nenhuma das três respostas está errada. O problema é outro: as três ficam na definição de superfície e nenhuma explica o mecanismo, que é o que a avaliação pede. Pelos critérios do próprio arquivo, o bloco não fecha:

| Critério | Situação |
|---|---|
| Todas as respostas têm justificativa, e não só o resultado | Parcial. Há um "porque" em cada uma, mas na 1 e na 3 ele é uma metáfora, não um mecanismo. |
| Pelo menos um exemplo do seu projeto ou dos exercícios | **Não cumprido.** Nenhuma resposta cita um repositório, um programa ou um bug seu. |
| Nenhuma resposta repete definição decorada sem explicar o mecanismo | **Não cumprido** nas perguntas 1 e 3. |

## Nota por pergunta

| # | Tema | Nota |
|---|---|---|
| 1 | Objetos do Git e voltar a qualquer versão | Raso, não passa |
| 2 | Step over x step into | Passa parcialmente (definição ok, exemplo fraco) |
| 3 | `cat \| grep \| wc -l` | Raso, não passa |

## O que passou

- **Pergunta 1:** "snapshot" é a palavra certa. O Git guarda o estado do projeto naquele momento, não só a diferença em relação ao anterior. Esse é o ponto de partida correto.
- **Pergunta 2:** a definição está correta. Step over executa a linha atual inteira, inclusive a chamada de método, e para na próxima linha do mesmo método. Step into entra no método chamado. Você também ligou o erro ao efeito: pular a chamada esconde o que acontece lá dentro.
- **Pergunta 3:** você identificou o papel de cada comando (`cat` lê, `grep` filtra, `wc` conta) e percebeu que o `|` é o que liga os três.

## O que ficou raso

**Pergunta 1. A pergunta era "no nível dos objetos" e você não citou nenhum objeto.**
- Faltou dizer o que um commit contém: um ponteiro para uma *tree* (o estado de todos os arquivos, que por sua vez aponta para os *blobs* com o conteúdo), mais o autor, a mensagem e o **pai** (o commit anterior).
- "São ligados pelos commit" é vago. O que liga um commit ao anterior é o ponteiro de pai guardado dentro dele. Você não disse isso.
- "Refazer o caminho de volta" descreve algo que o Git **não** faz. Isso sugere que você imagina que ele desfaz alterações uma a uma até chegar na versão antiga. Como cada commit aponta para uma tree completa, voltar a uma versão é só ler aquela tree. Não há nada para refazer. Esse é o ponto da pergunta "por que consegue voltar a qualquer versão", e você errou o mecanismo, mesmo com o resultado certo.
- Não apareceu a ideia de que os objetos são identificados pelo hash do conteúdo e por isso não mudam depois de criados. É isso que garante que a versão antiga continua intacta.
- Você também não disse nada sobre o que a branch é nesse modelo (um nome que aponta para um commit). Isso entra direto no Bloco 5.

**Pergunta 2. O exemplo é genérico.**
- "Talvez o bug estivesse dentro do método" é a definição repetida com outras palavras. A pergunta pedia um caso concreto, com código: qual linha, qual variável, o que você veria de diferente em cada escolha. Um exemplo meu: `total = calcularDesconto(pedido)` retorna um valor errado. Com step over, você só vê o valor ruim depois de ele ser atribuído. Com step into, você vê a variável que está errada *dentro* de `calcularDesconto`.
- Você só cobriu um lado do erro. Entrar em tudo também faz perder a causa: você acaba dentro do código de biblioteca (`String.format`, `ArrayList.add`), gasta tempo sem achar nada e perde a linha que importava. Não apareceu step out, que é a saída para esse caso.
- Não há menção a pilha de chamadas (*call stack*). É ela que explica o que o step into faz: empilha um novo frame, e o step over executa o método sem mostrar esse frame.

**Pergunta 3. Você nomeou os comandos, mas não explicou o mecanismo.**
- "Por conta da barra que funciona como um cano" é uma metáfora, não uma explicação. O mecanismo é este: a **saída padrão (stdout)** de um comando vira a **entrada padrão (stdin)** do próximo. O `grep` não sabe que o `cat` existe. Ele só lê o que chegar no stdin. Por isso programas pequenos e independentes se combinam.
- "O wc conta quantos tem" está impreciso. O `wc -l` conta **linhas**, não ocorrências. Se uma linha tiver `ERROR` duas vezes, ela conta uma vez. Se a pergunta fosse quantas vezes `ERROR` aparece, essa pipeline daria a resposta errada. Você não disse o que o `-l` faz.
- Você também não disse o que o `grep ERROR` casa: linhas que **contêm** o texto, diferenciando maiúsculas de minúsculas. `error` e `Error` não entram.
- O `cat` ali é desnecessário (`grep ERROR app.log | wc -l` dá o mesmo resultado). Não é erro, mas mostra o que você ainda não entendeu: o `grep` lê arquivo sozinho, então o `cat` só serve para ilustrar o pipe.
- A regra do arquivo diz "nas perguntas com código, diga o resultado antes de executar". Você não disse o que sairia (um número) nem registrou que executou. Se não rodou, rode agora.

## Onde eu decorei em vez de entender

- **"Cano de conexão"** (pergunta 3). É a analogia que aparece em qualquer tutorial, e você usou como se fosse a explicação. Se alguém perguntar "o que passa por esse cano?", você não respondeu. A resposta é stdout para stdin.
- **"Snapshot... histórico... ligados"** (pergunta 1). São as palavras da introdução do Git. A prova de que ficou na superfície é "refazer o caminho de volta", que contradiz o modelo de snapshots que você mesma citou. Se o Git guarda snapshots completos, ele não precisa refazer caminho nenhum.
- **A definição de step over/into** (pergunta 2) parece entendida, não decorada: você a conectou ao efeito no bug. Mas, sem um exemplo seu, não dá para confirmar. Um exemplo concreto resolveria.
- Você não escreveu "não sei" em nenhuma pergunta, e a regra pedia isso quando fosse o caso. Pelo que respondeu, na 1 você provavelmente não sabe o que é uma tree, um blob ou um ponteiro de pai, e na 3 não sabe o que é stdin/stdout. Aqui estão as lacunas que eu enxergo. Se você já sabia algo disso, a resposta não mostrou.

## O que revisar antes de avançar

1. **Objetos do Git.** Rode num repositório de teste:
   ```
   git cat-file -p HEAD
   git cat-file -p HEAD^{tree}
   git cat-file -t <hash de um blob>
   ```
   Depois explique, com as suas palavras, o que cada saída mostra e por que `git checkout <commit antigo>` não precisa "refazer" nada. Use a saída real do seu repositório como exemplo.
2. **stdin/stdout e pipe.** Rode `cat app.log | grep ERROR | wc -l` e, separado, `grep ERROR app.log | wc -l` e `grep -c ERROR app.log`. Depois crie um `app.log` com uma linha que tenha `ERROR` duas vezes e veja a contagem. Explique por que deu o resultado que deu.
3. **Step into x step over com um caso real.** Pegue o programa Java do exercício da prática 2. Ache uma chamada de método em que step over esconde a causa e outra em que step into te leva para código de biblioteca sem utilidade. Anote as linhas e os valores das variáveis que você viu em cada caso, e depois escreva o exemplo que a pergunta 2 pedia.
4. **Preencher o `resumo.md`.** Ele está em branco. O bloco previa 1h de fechamento para isso, e a seção "O que me confundiu" é onde as lacunas acima deveriam ter aparecido. Preencha-o antes de refazer a avaliação.
5. **Refazer as perguntas 1 e 3**, e a 2 com o exemplo concreto, citando um exemplo seu em cada uma. Sem consulta, desta vez com o "não sei" quando for o caso.

## Resposta rápida

Não avance para o Bloco 2 ainda. Seu entendimento do Git e do terminal tem a direção certa, mas é de superfície. Os itens 1 a 3 acima levam cerca de uma hora e são o que falta para fechar o bloco.
