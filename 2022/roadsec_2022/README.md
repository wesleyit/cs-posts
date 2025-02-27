# RoadSec 2022 - Back on the scene!

Eu adoro a cultura das comunidades de hacking, de makers, de cybersecurity em geral. O RoadSec é um dos eventos que eu mais gosto (junto com BSides e H2HC), e vem se tornando cada vez maior a cada ano. Depois de quase 3 anos sem evento, depois da pandemia, do mundo *digital-first*, do "Fulano, você esqueceu de tirar do mudo pra falar", a gente mal sabe como se comportar num evento com milhares de pessoas. Mas rolou, e pra mim foi muito legal.

Cada pessoa tem uma experiência diferente de acordo com as palestras que escolhe. Eu tento assistir com um olhar otimista, e se não consigo a profundidade que esperava, não hesito em procurar o palestrante para um bom papo.

Desta vez não foi diferente; já saí de casa com a minha lista de palestras pronta. Foi assim:



### Palestras (ordem cronológica)

#### 1. Keynote do Samy Kamkar

![Image](https://pbs.twimg.com/profile_images/1522373698119815168/NEKAvw_s_400x400.jpg)

O cara é inspirador. Ele contou um pouco da história dele no mundo de segurança, e mostrou pesquisas e projetos em IoT, cartões de crédito, carros, drones... Foi bastante inspirador. A frase mais legal que eu ouvi no evento foi do Samy:

> **O "S" em IoT é de Segurança.**

Faz todo o sentido! IoT pode gerar dores de cabeça se a gente esquece de incluir os devices no plano de segurança.

Recomendo demais o canal dele no Youtube: [samy kamkar - YouTube](https://www.youtube.com/channel/UC4m2G6T18_JcjwxwtwKJijw)

#### 2. Palestra Modelagem de Ameaças e Quebra de Controle de Acesso

Danilo Costa e Tiago Zaniquelli, Analistas de Segurança da Informação na Conviso Application Security

Os caras fizeram uma palestra mostrando o que é uma fraqueza (Common Weakness Enumeration - <https://cwe.mitre.org/>), como ela pode ser explorada e uma vulnerabilidade pode ser descoberta e registrada (Common Vulnerabilities and Exposures - <https://cve.mitre.org/>).

Eles mostraram com um evento real, um CVE descoberto pelo Danilo Costa em um hardware da Fortinet. Falaram bastante (dentro do que é possível em meia hora) sobre Broken Access Control. Mostraram como usar modelagem de ameaças para ter uma linha lógica de como proceder durante os testes até conseguir atingir o objetivo do ataque.

A palestra em si foi legal, mas o papo que puxei com eles depois da palestra foi ainda melhor. O Danilo me deu dicas de como iniciar na pesquisa de CVEs (tenho intenções acadêmicas).

Para saber mais sobre modelagem de ameaças, recomendo essa documentação da Microsoft: [Microsoft Security Development Lifecycle Threat Modelling](https://www.microsoft.com/en-us/securityengineering/sdl/threatmodeling)

#### 3. Palestra Avengers, disassemble!

Daiane Santos, Engenheira de Segurança Mobile no Nubank

A Daiane mostrou algo bem real, que faz parte do nosso cotidiano: como um pacote APK (formato utilizado pelo sistema Android) é organizado por dentro e como isso pode dar dor de cabeça quando as melhores práticas de segurança não são seguidas no app. Detalhes como as telas que podem ser executadas diretamente por outros apps, abuso de permissões, e muito mais. Mostrou uma ferramenta chamada MobSF (<https://github.com/MobSF/Mobile-Security-Framework-MobSF>) que facilita bastante o trabalho de extrair o APK e buscar os arquivos no pacote.

Para quem quer um resumo da palestra e mais links para se aprofundar, ela deixou um link bem completo: <https://wh0isdxk.github.io/>.

#### 4. Palestra Realizando Threat Hunting com o MITRE Attack Framework

Guilherme Almeida, Engenheiro de Segurança Ofensiva na CloudWalk

Esse assunto é recente para mim; ouvi falar de MITRE Attack (<https://attack.mitre.org/>) pela primeira vez em uma conversa com o grande Flavio Honda (<https://www.linkedin.com/in/flavio-honda/>). Para minha surpresa, o framework existe há quase uma década.

Attack Significa Adversarial Tactics, Techniques & Common Knowledge – Táticas, Técnicas e Conhecimento Comum de Adversários, e é um grande compilado de observações que o MITRE fez em ataques reais.

![](assets/README/9a1efa2dd20b6fe2888101a066b4ef0ba0c2aaac.png)

Cada etapa de um ataque é descrita com técnicas, detalhes, ferramentas, e é possível usar o framework para organizar um ataque de Red Team, por exemplo. É um recurso precioso para quem estuda técnicas de intrusão.

#### 5. Palestra Implante NFC LED - DYI Biohacking, seu corpo como ambiente de teste

Matheus Gaboardi, Security Focal na Kyndryl

Essa palestra foi um interesse particular. Eu tenho 3 implantes: um chip criptográfico, um chip MIFARE e um chip duplo com Ultralight + RFID. É legal ouvir as experiências, descobertas e dificuldades de quem também curte esse tipo de BioHacking. Peguei o contato do Matheus para conversarmos mais sobre implantes :D

Para quem tem interesse, comprei meus implantes desta empresa: https://dangerousthings.com/

#### 6. Palestra Hardware Witchcraft, the cult of fault injection

Julio Della Flora, Líder Técnico de Red Team na Locaweb

E chegou a palestra que eu mais gostei em todo o evento! O Julio <https://www.instagram.com/juliodellaflora/> é absurdo. O Lucas Teske <https://lucasteske.dev/> também é incrível, não palestrou diretamente mas foi recomendado pelo Julio durante a conversa.

A mensagem chave da palestra é que quando um processador estiver trabalhando e você mexe com ele de formas inesperadas, o processamento pode ser alterado. Por exemplo, se quando um processador for comparar a senha que você digitou com a senha correta em um banco de dados, você cortar por um curtíssimo período de tempo a energia deste processador, ele pode "pular" a instrução que faz a comparação, permitindo seu login. O Julio trouxe exemplos reais da aplicação dessa técnica, como por exemplo o desbloqueio do Nintendo Switch.

Vale a pena DEMAAAAIISSSS ver os vídeos do canal do Julio, e eu com certeza vou pesquisar mais sobre o assunto e tentar reproduzir alguns experimentos em casa.

Acessa lá: [Ataques de Fault Injection, Saiba Como Isso Funciona na Prática! - YouTube](https://www.youtube.com/watch?v=20qMSG07hAs)

### Livros

Aproveitei as promoções para comprar alguns livros de tecnologia. Paguei preços mais baixos que nas lojas, a maioria destes livros eu já vinha acompanhando e achei a oportunidade ótima.

#### [Future Crimes: Tudo está conectado, todos somos vulneráveis e o que podemos fazer sobre isso | Amazon.com.br](https://www.amazon.com.br/Future-Crimes-Conectado-Vulner%C3%A1veis-Podemos/dp/8567389496)

![](https://images-na.ssl-images-amazon.com/images/I/416OY9p+mfS._SX353_BO1,204,203,200_.jpg)

Esse é basicamente um livro de terror. O Marc Goodman conta histórias reais de ataques pouco triviais, se aproveitando de tecnologias muito recentes que ainda tem poucos recursos de proteção.

#### [Livro de Blockchain Ethereum - Casa do Código](https://www.casadocodigo.com.br/products/livro-blockchain-ethereum)

![Livro de Blockchain Ethereum](https://cdn.shopify.com/s/files/1/0155/7645/products/p_f77147f5-25b8-44e8-96eb-f810eb70542b_large.jpg?v=1646681073)

Eu tenho uma visão superficial de Blockchain, e espero conseguir aprender mais a fundo com este livro.

#### [Livro Aprofundando em Flutter - Casa do Código](https://www.casadocodigo.com.br/products/livro-aprofundando-flutter)

![Livro Aprofundando em Flutter](https://cdn.shopify.com/s/files/1/0155/7645/products/Aprofundandoemflutter_Amazon_large.jpg?v=1631564172)

Para quem faz protótipos, gosta de testar hipóteses ou mesmo transformar ideias do papel em realidade, Flutter é uma das melhores pedidas. Já fiz alguns apps em Flutter, mas espero subir um patamar com este material.

#### [Livro de Web Semântica - Casa do Código](https://www.casadocodigo.com.br/products/livro-web-semantica)

![Livro de Web Semântica](https://cdn.shopify.com/s/files/1/0155/7645/products/IntroducaoaWebSemantica_ebook_large.jpg?v=1631717954)

Quando eu fiz o MBA de Data Science na FIAP, conheci o tema Web Semântica pela primeira vez com a incrível Dra. Regina Cantele <https://www.linkedin.com/in/regina-cantele-86a169/>, uma das maiores especialistas no campo. Infelizmente o tempo de aula foi curto, e este livro vai me ajudar a saber mais.

#### [Livro de Sistemas reativos - Casa do Código](https://www.casadocodigo.com.br/products/livro-sistemas-reativos)

![Livro de Sistemas reativos](https://cdn.shopify.com/s/files/1/0155/7645/products/p_22f9a726-5a8a-48f3-a6b5-3cd78fe8e10d_large.jpg?v=1631283564)

Eu já queria aprender mais sobre o tema. Quando peguei o livro na mão, achei super engraçado. Juntou a faca e o queijo.

### Rolês

Passeando pelo evento, encontrei o M4v3r1ck (Helvio Junior), da Sec4US (<https://sec4us.com.br/>). Os videos dele já me ajudaram muito, como esse aqui: [Buffer Overflow - Explorando a vulnerabilidade Sudo CVE-2019-18634 - YouTube](https://www.youtube.com/watch?v=rpqMHnaTk98)

Também vi meus amigos Jampa (Centauro), Gabs e Ane (AWS), conheci um monte de gente nova e adicionei os contatos.

### Perrengues

Na edição anterior do evento, você pegava um cartãozinho, colocava crédito em um dos muitos pontos disponíveis para recarga e pronto! Podia comprar qualquer coisa com o crédito. Este ano foi diferente. Tinha uma área enorme com algumas opções de comida, mas você tinha que comprar as fichas antes nos caixas. O problema é que tinha poucos caixas, e você tinha que comprar antecipadamente exatamente o que queria. Por exemplo, você tinha que comprar uma ficha de X-Burger, uma de Batata com Bacon e uma de cerveja comum. Se na hora quisesse mudar para X-salada ou Batata com Queijo, não podia. Esse sistema foi bem ruim, tirou a flexibilidade e causou filas quilométricas. Não tinha bebedouro, quem queria água tinha que perder mais de 30 minutos no caixa e outros 15 na fila do bar. Isso foi mancada.

Só tinha 1 trailer vendendo hamburguer. Comprei 2 fixas de hamburger mas não comi, senão teria perdido palestras importantes. Sorte que o cara da batata trocou para mim, mas acabei saindo no prejuízo, e passei o dia com batata frita, nada saudável.

As filas de algumas atrações (stand do C6, chopeira da BTG, entre outros) também estava impraticável.

Acho que o grande fato que isso mostra é que o evento cresceu, os organizadores, expositores e patrocinadores precisam pensar em escala agora. E isso é uma prova do sucesso do evento.

![](https://lh3.googleusercontent.com/WPu4LdV9_qnjnGj1u50d-qN5QpQDy9EYmP07JDoRoqCP4OQQYfzB9hntAkamh5bVAh4Aw4nmgqkZhw-Ae86pm7SBPOHTLevTtVGG9otKiR-mQenQ0IAuM4dX18ScvzVVBAaHJYACC_L5RTLt9XYsDIk4coeWQSwnZXPKWgcaEwjjhTZjcUh0efMzVhR03KbTXJ_aXuZx8RM_rIk00rcc0EvM6c7DoRnfG56CIA9zTbVdZuIBVAORTudRPAmDnj23_CZQBVw6FF7vj2dt3TOGUdkpqMDVBW7V40okCSTlFT5BVcqZTiOZfikWU5et450xMUPhRpQgSYIqMc6ZCe-P1rEK9Cc2ukmfhRUigyt_2YOCtPGkMdDwYyOJDP7optg2IiKacAIPf_ji4-rvIHP6NWnvHfvvCM0Q-y-bXeix65inG59cYopu1j0HQuLTw5qWM5Aq2aiLVUrZZMxdlNxpDzCgiP2dxY5xcgeri-5dpoSnQmKV2ewpT5Lgc8_rf7KBMzK_hHg0JsGGFGehN-9hkqfNM49KpwfplFfpP9aS2AtQBS9-oVFAzM9KiMSlXd5aGlLYrZwfpi_XAA3ZvHKjlkMY6eQI-ALSBVIz42vZnF1-ei5nduA9UnOTRufUGds6yOtFS_wIM08Cd2ooVX5Pxjs2z75lqKZ67VfX2PBAQ7asaXyz1v0CprlXOKfEHRhCmBmxHegg_eBv6bqQi_X1_pyuQzYInbu1AS5-2ymdTh4qwBuSxncDLjDj7xMz=w1921-h553-no?authuser=0)



### Poderia Melhorar

As oficinas diminuíram. Eu gostava do modelo anterior, com muito mais espaço pra oficinas e comunidades. Não teve lockpicking, Software Defined Radio, entre outras coisas legais.

Faltou também o pessoal de implantes de chips, tipo a Dangerous Things ou outros. Eu teria colocado mais um chip, certamente, rsrs.



### Mas e aí?

Foi incrível. Aproveitei demais e recomendo para quem nunca foi, é um evento delicioso se você souber aproveitar. Ansioso pela H2HC...


