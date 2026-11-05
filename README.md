# Roadmap: fundamentos de engenharia backend

Um roadmap de 20 semanas (cerca de 5 meses, até 5 horas por semana) para dominar os fundamentos de backend **sem depender da IA para escrever código**: entender por que cada coisa acontece e diagnosticar sozinha onde e por que algo deu errado.

Ele é a base para estudar System Design depois. System Design só faz sentido quando você entende o que acontece dentro de um único serviço.

## Ponto de partida

- **Hoje:** Engenheira de Software Júnior (backend Java) e estagiária de Engenharia de IA (Go e Python), cursando Sistemas de Informação.
- **Nível atual em Java sem IA:** consigo fazer uma API simples, mas não entendo o que acontece por baixo.
- **Gap principal:** entender o porquê das coisas e diagnosticar erros sozinha.
- **Tempo:** até 5 horas por semana, em paralelo com trabalho e faculdade.

## As etapas

| Etapa | Semanas | Foco | Tema |
|---|---|---|---|
| [1](etapa-1/README.md) | 1 a 4 | Entender | Java e ferramentas |
| [2](etapa-2/README.md) | 5 a 8 | Entender por baixo | Estruturas de dados, memória e concorrência |
| [3](etapa-3/README.md) | 9 a 12 | Rodar e modificar | HTTP, Spring e testes |
| [4](etapa-4/README.md) | 13 a 16 | Diagnosticar | Banco de dados e ambiente |
| [5](etapa-5/README.md) | 17 a 20 | Defender | Observabilidade, incidentes e defesa final |

Cada etapa depende da anterior. O projeto integrador atravessa todas elas.

## Como usar

1. **Antes de começar:** leve este plano ao seu mentor com as perguntas de [`perguntas-mentor.md`](perguntas-mentor.md) e ajuste o plano com o Prompt 2 do método.
2. **A cada semana**, abra a pasta do bloco e siga esta ordem:
   - `conteudo.md`: estude e faça a prática.
   - `resumo.md`: anote o que aprendeu, com as suas palavras.
   - `avaliacao.md`: responda sem consulta.
   - `feedback.md`: registre a correção feita com o Prompt 4 abaixo.
3. **Marque o avanço** em [`progresso.md`](progresso.md).
4. **Se uma semana não for suficiente**, use duas. É melhor atrasar do que avançar com a base frágil.

## Prompt 4: ser avaliada ao fim de cada bloco

```
Terminei o bloco [nome]. Segue meu resumo:

[cole seu resumo.md preenchido]

Seguem minhas respostas:

[cole sua avaliacao.md respondida]

Me avalie usando o avaliacao.md deste bloco. Seja rigoroso:
- Resposta certa sem justificativa não passa
- Aponte onde eu decorei em vez de entender
- Se eu não souber algo, quero saber disso agora, não no final

Escreva o resultado no formato do feedback.md: o que passou, o que ficou raso,
e o que eu preciso revisar antes de avançar para a próxima etapa.
```

## Regras para usar IA durante o roadmap

- **A IA é professora, não autora.** Escreva o código primeiro, mesmo que fique ruim. Quando travar, peça uma explicação do conceito ou do erro, e não a solução.
- **Nenhuma linha que você não consiga explicar** entra no projeto.
- **Leia o erro antes de perguntar.** Tente localizar a linha e entender a mensagem do stack trace sozinha.
- **Nunca cole código ou detalhes internos do trabalho** (nomes de sistemas, arquitetura, bibliotecas proprietárias) em uma IA. Essas dúvidas vão para o mentor ou para colegas.

## Fora do escopo (e por quê)

Este roadmap cobre os fundamentos de um único serviço. Ficam de fora, de propósito:

- **System Design e sistemas distribuídos** (Saga, Outbox, Kafka, microsserviços): é a próxima fase, e ela depende de tudo o que está aqui.
- **Kotlin e Go:** ficam mais fáceis depois de dominar Java a fundo. Kotlin roda na mesma JVM, então quase tudo daqui se aplica a ele.
- **Cloud, AWS e Kubernetes:** são camadas de infraestrutura sobre os conceitos de containers e ambiente que você vai aprender aqui.
- **Frontend:** não é o foco da sua carreira backend.
- **IA e LLMs:** você já tem prática no trabalho, e o objetivo aqui é justamente construir a base sem eles.

## Estrutura

```
roadmap/
├── README.md
├── progresso.md
├── modo-sabotagem.md
├── perguntas-mentor.md
├── etapa-1/ … etapa-5/
│   ├── README.md
│   └── bloco-NN/
│       ├── conteudo.md
│       ├── resumo.md
│       ├── avaliacao.md
│       └── feedback.md
└── projeto-integrador/
    ├── README.md
    ├── fase-1.md … fase-5.md
    └── avaliacao-final.md
```
