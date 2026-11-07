# Roadmap: fundamentos de engenharia backend

Um roadmap de 27 semanas (cerca de 6 a 7 meses, até 5 horas por semana) para dominar os fundamentos de backend **sem depender da IA para escrever código**: entender por que cada coisa acontece e diagnosticar sozinha onde e por que algo deu errado.

Ele é a base para estudar System Design depois. System Design só faz sentido quando você entende o que acontece dentro de um único serviço.

## Ponto de partida

- **Hoje:** Engenheira de Software Júnior (backend Java) e estagiária de Engenharia de IA (Go e Python), cursando Sistemas de Informação.
- **Nível atual em Java sem IA:** consigo fazer uma API simples, mas não entendo o que acontece por baixo.
- **Gap principal:** entender o porquê das coisas e diagnosticar erros sozinha.
- **Tempo:** até 5 horas por semana, em paralelo com trabalho e faculdade.

## As etapas

| Etapa | Semanas | Foco | Tema |
|---|---|---|---|
| [1](etapa-1/README.md) | 1 a 5 | Entender | Java, ferramentas e trabalho em time |
| [2](etapa-2/README.md) | 6 a 9 | Entender por baixo | Estruturas de dados, memória e concorrência |
| [3](etapa-3/README.md) | 10 a 15 | Rodar e modificar | HTTP, Spring, testes e segurança |
| [4](etapa-4/README.md) | 16 a 21 | Diagnosticar | Banco de dados, idempotência e ambiente |
| [5](etapa-5/README.md) | 22 a 27 | Defender | Migrações, código herdado, incidentes e defesa final |

O plano soma cerca de 130 a 140 horas. A versão 2, depois da validação com o mentor, está descrita no [`CHANGELOG.md`](CHANGELOG.md).

## O que mais importa

Segundo o mentor, estes são os pontos que mais diferenciam um engenheiro júnior de um pleno, em ordem. Quando faltar tempo, priorize as atividades ligadas a eles:

1. Método de diagnóstico: hipótese e evidência, nunca tentativa e erro.
2. Transações e concorrência.
3. Localizar em que camada está o erro.
4. Escrever o teste que falha quando o código quebra.
5. Ler `EXPLAIN` e métricas.
6. Defender um trade-off.

Implementar estruturas de dados na mão, por outro lado, não diferencia. Por isso o roadmap só tem uma.

Cada etapa depende da anterior. O projeto integrador atravessa todas elas.

## Como usar

1. **Validação:** feita (veja o [`CHANGELOG.md`](CHANGELOG.md)). Se mudar algo grande no plano, valide de novo com o mentor.
2. **A cada semana**, abra a pasta do bloco e siga esta ordem:
   - `conteudo.md`: estude e faça a prática.
   - `resumo.md`: anote o que aprendeu, com as suas palavras.
   - `avaliacao.md`: responda sem consulta.
   - `feedback.md`: registre a correção feita com o Prompt 4 abaixo.
3. **Marque o avanço** em [`progresso.md`](progresso.md).
4. **Se uma semana não for suficiente,** continue o bloco na semana seguinte, no mesmo ritmo de 5 horas, e empurre o prazo final. **Nunca dobre as horas de uma semana para recuperar.** Isso gera cansaço e estudo raso.

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

- **System Design e sistemas distribuídos** (cache, filas, consistência eventual, replicação): é a próxima fase, descrita em [`proxima-fase.md`](proxima-fase.md).
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
├── CHANGELOG.md
├── proxima-fase.md
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
