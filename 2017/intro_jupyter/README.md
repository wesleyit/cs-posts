Introdução ao Python com Jupyter
================================

> Aviso aos hackers de plantão: este é um post para iniciantes com conceitos
> básicos. Se você já domina as artes obscuras do Python, volte em alguns dias
> para a parte II, analisando dados com `Pandas` e `Sklearn`. :)

Então você quer mexer com Python? Boa escolha. É uma linguagem bem bacana,
e tem um jeito bem legal de começar: usando seu browser. Graças ao
[Jupyter](http://jupyter.org). Mas vamos chegar lá daqui a pouco.


Instalação
----------

Vamos começar instalando os pacotes. Se você usa Linux, provavelmente já
tem o Python de fábrica. Mas sempre acaba faltando alguma coisa, então vamos
dar a receitinha de bolo. Além do Python, queremos o `pip` e o `virtualenv`,
que como veremos adiante, facilitam demais a vida.


### No Linux (Debian based)

```
$ sudo apt-get update
$ sudo apt-get install -y python3-pip build-essential \
  libssl-dev libffi-dev python-dev python3-venv
```

### No Mac
`$ brew install python3`

Pronto! A partir de agora vamos utilizar o `pip` para instalar os pacotes do
Python que nossos projetos exigirem. Isso será feito em uma pasta específica
para cada projeto, que chamaremos de ambiente virtual, ou **virtual env**.


Hello World
-----------

Vamos começar nosso `hello_world` (para mais detalhes sobre nomenclatura de
arquivos, classes e variáveis em Python, leia o
[PEP8](https://www.python.org/dev/peps/pep-0008), que é o principal guia
de estilo da linguagem). Seguiremos o seguinte roteiro:

1. Criar uma pasta para o nosso projeto.
2. Criar um ambiente virtual.
3. Ativa o ambiente virtual.
4. Criar o `hello_world`.
5. Executar o `hello_world`.

```shell
$ mkdir learning_python    ## cria a pasta
$ cd learning_python    ## entra na pasta
$ virtualenv -p python3 env    ## cria o amviente virtual com python3 na pasta env
$ source env/bin/activate    ## ativa o ambiente virtual
$ atom hello_world.py  ## use o seu editor favorito :D
```

O conteúdo do arquivo deve ser algo como:

```python
#!/usr/bin/env python
print("Hello, World!!!")
```

Para executar, podemos fazer de duas formas:
a. Chamando o Python passando o arquivo como argumento:

```shell
$ python hello_world.py
Hello, World!!!
```

b. Ou dando permissão de execução e chamando o script diretamente:

```shell
$ chmod a+x hello_world.py
$ ./hello_world.py
Hello, World!!!
```
Aeeeeeee! Parabéns, agora você já não é mais um inexperiente no Python.
Vamos avançar para o Jupyter?
