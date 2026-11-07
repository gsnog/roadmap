# CHANGELOG

## Versão 2: ajustes após validação com o mentor

### Prazo

- **De 20 para 27 semanas** (cerca de 6 a 7 meses). O mentor estimou de 130 a 140 horas de trabalho real, e não 100, porque alguns blocos tinham de 7 a 10 horas de material e as fases do projeto se somam.
- **Regra nova:** se um bloco atrasar, ele continua na semana seguinte e o prazo final é empurrado. Nunca se dobram as horas de uma semana para recuperar.

### Cortes

- **Bloco 1** reduzido para caber em 5 horas: saíram o Pro Git (foi para o bloco 5) e o exercício de conflito de merge.
- **Etapa 2:** saíram a leitura sobre grafos, dois dos três problemas do LeetCode do bloco de árvores, os capítulos 3 em diante de *Java Concurrency in Practice* (ficaram só os capítulos 1 e 2) e a profundidade em tuning de garbage collector (agora é leitura por cima).

### Acréscimos

- **JUnit básico antecipado para o bloco 2,** porque a Fase 1 do projeto já exige testes. O bloco de testes da etapa 3 virou aprofundamento.
- **Bloco 5, Git colaborativo, code review e CI:** pull requests, dar e receber review, GitHub Actions rodando os testes e comunicação técnica escrita.
- **Bloco 14, autenticação e autorização mínimas:** API key e regras de papel.
- **Bloco 19, idempotência e retries,** com entrega na Fase 4.
- **Bloco 23, migração de schema com dado vivo,** na transição da Fase 4 para a 5.
- **Bloco 24, código herdado e comunicação técnica assíncrona,** incluindo o estudo de um sistema real com os critérios do mentor.
- **Blocos 15 e 21, semanas de projeto,** para absorver o tempo das Fases 3 e 4.
- **Seção "O que mais importa" no README,** com as prioridades do mentor.
- **Sabotagem com uma pessoa:** a rodada do bloco 26 e a defesa final passam a ser obrigatoriamente com uma pessoa.
- **Arquivo `proxima-fase.md`,** com o caminho para System Design.

### Onde a IA discordou do mentor (e o que foi feito)

- **Implementar estruturas na mão.** O mentor disse que isso não diferencia um júnior de um pleno, e a IA concorda. Mesmo assim, foi mantida **uma** implementação: a tabela hash do bloco 6, de cerca de 1 hora. O motivo é que o objetivo deste roadmap não é só a carreira, mas entender o porquê das coisas, e a tabela hash explica diretamente o funcionamento do `HashMap`, as colisões e o bug de `equals` sem `hashCode` do bloco 3. A pilha e a fila foram cortadas.
- **Autenticação.** O mentor citou a autenticação mínima como algo que falta e, no projeto, como opcional. Ela foi incluída como obrigatória, mas mínima (API key e dois papéis), porque já tem um bloco de estudo dedicado e o custo extra no projeto é pequeno.
