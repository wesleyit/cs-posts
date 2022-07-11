Descomplicando as Redes Neurais
===============================

Olá, que bom ver você aqui mais uma vez! Hoje o assunto é **Inteligência Artificial**. Este é um campo de estudo bem amplo, mas com certeza uma das partes da IA que fazem mais sucesso são as **Redes Neurais Artificiais**. Vamos dar uma introdução descomplicada e direta sobre o que são, onde vivem, do que se alimentam e como podemos utilizá-las nos nossos programas.
Também vamos olhar exemplos usando algumas bibliotecas bem legais, como Sklearn, TFLearn e Tensorflow, todas em Python. Ah, e se você não tem PHD em matemática, não se preocupe ;-)

Temos visto carros autônomos, lojas virtuais que escolhem os produtos por você, diagnóstico automatizado e rápido de doenças por exames de imagem, seleção de músicas baseadas em humor, recomendação de filmes... a lista não para de crescer, e sempre ouvimos falar que essas "novidades quentes" tem um tipo de rede neural por baixo do capô.

Mas "que diabos é uma rede neural"???

Uma rede neural é uma maneira de escrever um programa de modo que ele tome uma decisão imitando a forma como o neurônio do cérebro toma decisões. Ajudou? Não muito? Calma :-)

Tem gente que **AMA** chocolate. :chocolate_bar: :heart_eyes: :chocolate_bar:
O que acontece na cabeça delas quando elas comem chocolate?

[desenho1]

Quando o chocolate toca a língua, pequenas papilas gustativas reagem imediatamente.

[desenho 2]

Olhando mais de perto, vemos que o chocolate faz com que essas papilas enviem sinais elétricos ao cérebro através de longos nervos. É como se fossem inúmeros fios ligando sua língua ao seu centro de prazer no cérebro.

[desenho 3]

Vamos agora pensar no neurônio. É uma coisinha com várias entradas e apenas uma saída. Se os impulsos elétricos nas entradas forem fortes o bastante, haverá um sinal na saída desse neurônio, e dizemos que ele foi **ativado**, liberando um balde de serotonina (prazer!!!) para quem comeu o delicioso chocolate. O princípio é simples, varias entradas, uma saída que depende dessas entradas. No cérebro temos vários neurônios conectados, controlando as mais diferentes reações do nosso corpo.

Em uma rede neural artificial a coisa toda é bem parecida.

Vejamos um exemplo de um controlador de ar condicionado. Sabemos que a sensação de calor que sentimos está ligada à relação entre temperatura e umidade.

Neste caso, temos um sensor de temperatura e um sensor de umidade
ligados a um computador que utiliza uma rede neural para decidir
se liga ou não o ar condicionado.

[desenho-ar-1]

A temperatura aqui está média e a umidade está baixa. Combinadas, elas não produzem estímulos suficientes para ativar a rede neural e ligar o ar condicionado.

[desenho-ar-2]

Agora a umidade também subiu, atingindo um valor que ultrapassa o limiar da rede, ativando o neurônio e ligando o ar condicionado.

Normalmente um neurônio artificial recebe um monte de informações. Ele junta todas elas para tomar sua decisão. Para algumas informações ele dá mais importância, para outras menos, e isso é o que chamamos de **pesos**. Por exemplo, quando eu vou comprar um produto no mercado, levo em consideração o preço, a qualidade, minha necessidade, mas no final das contas o que mais importa é o preço, afinal, se for mais caro do que posso pagar, não tenho como comprar. E é assim que fazemos o neurônio artificial aprender: ajustamos os pesos de suas entradas para que as informações mais relevantes influenciem mais na saída.

[desenho-neuronio]

Todas as entradas são multiplicadas pelos seus pesos e depois são somadas. O resultado disso é entregue para a parte que cuida da decisão, que chamamos de **função de ativação**. Podemos usar várias saídas diferentes: saídas que geram 0 ou 1, saídas entre 0 e 1, entre -1 e 1, entre -infinito e infinito... tudo vai depender do que queremos fazer com essa informação. Quando queremos uma decisão, é útil ter 0 ou 1. Quando queremos uma nota ou classificação, é útil ter um número decimal entre 0.0 e 1.0 como saída.

Tá, falamos de neurônios, mas e as redes? Fácil. É só colocar um monte de neurônio em camadas, desse jeito:

[rede]

Olhando as redes neurais mais de perto veremos que nem sempre precisamos de uma rede de verdade. Isso depende muito da natureza do problema. Quando falamos em Deep Learning, por exemplo, estamos tentando resolver problemas complexos com inúmeras variáveis, o que requer redes com muitos neurônios dispostos em várias camadas. Há problemas mais simples que podem ser resolvidos com um único neurônio. 

A teoria está legal, mas vamos à prática.

