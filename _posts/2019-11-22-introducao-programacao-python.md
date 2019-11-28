---
layout: post
title: "Introdução a Python automatizando a organização de arquivos"
categories: ['Manutenção']
authors: ['Alexandre Prestes']
tags: ["programação", "python", "introdução", "os", "arquivos"]
description: 'O artigo apresenta a linguagem Python e desenvolve um projeto para a organização de arquivos do computador.'
image: code.jpg
---
 
# Sumário
- Introdução
- Instalação
- Variáveis
- Listas
- Operadores
- Condições
- Repetições
- Projeto
- Referência
 
 
# Introdução
Pode-se definir programação de computadores como o processo de escrita de instruções,que ordenará um computador a como proceder. Essas instruções constituem um programa, para suprir determinada necessidade. Tal necessidade inclui, por exemplo, a automação de alguma tarefa ou o entretenimento em algum jogo. Para isso, essa escrita deve ser feita através de uma linguagem de programação, como C, Java, Ruby ou PHP.
 
Além dessas, uma linguagem bastante popular atualmente é o Python, que surgiu em 1991, criada por Guido van Rossum. Trata-se de uma linguagem poderosa e de fácil aprendizado. Ela é utilizada desde projetos Web até de Inteligência Artificial. Sua filosofia prega a simplicidade e a legibilidade do código. Isso está explícito em seu Zen, escrito por Tim Peters. Segue alguns itens da filosofia:
 
* Bonito é melhor do que feio.
* Simples é melhor do que complexo.
* Legibilidade conta.
* Se a implementação é difícil de explicar, é uma má ideia.
* Deve haver um - e preferencialmente só um - modo óbvio para fazer algo.
 
Neste artigo, será feita uma rápida apresentação da linguagem Python, com a finalidade de elaborar um projeto para a organização arquivos do computador.

---
# Instalação 
O Python pode ser baixado facilmente em seu [site oficial](https://www.python.org/) para Windows e MacOS. No Linux, as distribuições mais populares já possuem o Python instalado, então não é necessário se preocupar. Atualmente, a versão mais recente é a 3.8. 

Para verificar o sucesso da instalação, abra um terminal e digite `python3`. Python é uma linguagem interpretada, então o seu interpretador será aberto. Digite: 

```python
>>> print("Olá, mundo!")
```

O interpretador deve escrever no terminal:

```
Olá, mundo!
```

Para escrever scripts em Python, crie um novo arquivo em alguma pasta do computador, utilize algum editor de código e o execute pelo terminal:

```
python3 nome-do-script.py
```

---
# Variáveis
Variáveis são estruturas que armazenam valores em uma área da memória do computador. Inicialmente, esses valores são números, textos ou tipo lógico (True ou False). Para criar uma variável, basta inserir seu nome, o símbolo de igualdade e o valor.
 
Veja um programa que pede o nome do usuário e o exibe na tela. Nesse programa, a função `print` tem o papel de exibir algo, no caso o texto e o nome. Já a função `input` é responsável por ler o que o usuário digita em seu teclado.
 
```python
nome = input("Digite o seu nome: ")
print("Olá " + nome)
```
 
Agora, veja os valores possíveis de se armazenar em uma variável.
 
```python
inteiro = 10
flutuante = 10.8
 
casa = "casa"
dez = "10"
 
verdadeiro = True
falso = False
```
 
Variáveis são mutáveis, ou seja, elas podem ter seus valores alterados durante a execução do programa. No próximo exemplo, a função `print` exibirá primeiramente _10_ na tela, e na sua segunda chamada exibirá _olá_.
 
```python
v = 10
print(v)
 
v = "olá"
print(v)
```
 
---
# Listas
Também é possível armazenar mais de um valor em uma mesma variável. Para isso, são utilizadas variáveis compostas, como as listas.
 
```python
comida = ["carne", "arroz", "feijão"]
números = [10, 20, 30, 40, 50]
```
 
No próximo código, `#` representa um comentário. Tudo o que é escrito após esse símbolo é ignorado pela linguagem. Comentários são utilizados para fazer anotações no código, de modo a explicar a lógica das linhas seguintes. Use-os com moderação. Nesse caso, o comentário representa a saída (_output_) daquela linha.
 
Para acessar apenas um elemento da lista, usa-se o nome da variável, e a posição do elemento na lista. Note que o primeiro elemento tem posição/índice zero.
 
```python
comida = ["carne", "arroz", "feijão"]
print(comida[0]) # carne
print(comida[2]) # feijão
```
 
Adiciona-se valores a listas com o método `append`, da seguinte forma:
 
```python
lista = []
 
comida = input("Digite algo saboroso: ") # pudim
lista.append(comida)
print(lista) # [pudim]
```
 
---
 
# Operadores
As linguagens de programação podem ser utilizadas para fazer cálculos. Veja o exemplo que demonstra o uso das principais operações matemáticas:
 
```python
a = 10
b = 20
 
print(a + b)  # Soma
print(a - b)  # Subtração
print(a * b)  # Multiplicação
print(a / b)  # Divisão
print(a // b) # Divisão inteira
print(a % b)  # Resto da divisão
```
 
Além desses, existem os operadores relacionais. Eles retornam verdadeiro ou falso.
 
```python
a = 3
b = 9
 
print(a > b)   # Maior        - False
print(a >= b)  # Maior igual  - False
print(a < b)   # Menor        - True
print(a <= b)  # Maior igual  - True
print(a == b)  # Igual        - False
print(a != b)  # Diferente    - True
```
 
Por fim, os operadores lógicos, que são _and_(e), _or_(ou) e _not_(não):
```python
a = True
b = False
 
print(not a)   # False
print(not b)   # True
 
print(a and b) # False
print(a or b)  # True
```
 
Esses três operadores possuem tabelas, veja-as:
 
A | B | A and B
--- | --- | ---
True | True | True
True | False | False
False | True | False
False | False | False
 
A | B | A or B
--- | --- | --- |
True | True | True
True | False | True
False | True | True
False | False | False
 
A | | not
--- | --- | ---
True | | False
False | | True
 
# Condições
Condições são utilizadas para determinar quando um trecho de código deve ou não ser executado.
 
Por exemplo, imagine que um usuário diga que nasceu em 1998. Assim, sua idade será 21 anos (durante a escrita deste artigo). Por ter idade superior a 18, será informado que é maior de idade. Porém, caso tivesse a idade inferior a 18, seria informado que é menor de idade. Trata-se de um **if-else**, onde **if** significa _se_ e **else** _senão_.
 
O código a seguir corresponde a esse raciocínio. Perceba que caso a idade seja 21, apenas as cinco primeiras linhas seriam executadas pelo computador. Caso a idade fosse menor que 18, apenas as linhas 1, 2, 3, 4 e 7. As demais linhas são ignoradas.
 
```python
nascimento = int(input("Ano de nascimento: "))
atual = 2019
idade = atual - nascimento
if idade >= 18:
  print("Maior de idade.")
else:
  print("Menor de idade.")
```
 
No caso de mais condições, é possível usar `elif`. Essa estrutura corresponde a um **else-if**.
```python
código = 2
if código == 1:
   print("Pizza")
elif código == 2:
   print("Alface")
elif código == 3:
   print("Tomate")
else:
   print("Código inexistente")
```
 
---
# Repetições
Repetições são utilizadas para executar o mesmo trecho de código diversas vezes. Caso a necessidade seja escrever cinco vezes na tela _Olá, mundo_, uma forma de fazer isso seria:

```python
print("Olá, mundo")
print("Olá, mundo")
print("Olá, mundo")
print("Olá, mundo")
print("Olá, mundo")
```

Entretanto, uma única linha se repete cinco vezes. E caso se repetisse cem vezes? Seria trabalhoso escrever cem linhas iguais. Uma forma de resolver isso é utilizar repetições, com a estrutura `while`.

```python
começo = 1
fim = 100
while começo <= fim:
    print("Olá, mundo")
    começo = começo + 1
```

Ou então, por `for`, que é capaz de iterar (repetir) a partir de listas:

```python
for começo in range(1, 101):
  print("Olá, mundo")
```

`range(1, 101)` retorna uma lista com 100 elementos. Note que o intervalo é aberto, portanto a lista é de 1 até 100 (101 - 1).

---
# Projeto
Python é bastante utilizado para a automação de tarefas, pois possui vantagem ao ser multiplataforma, ou seja, funciona em diversos sistemas (Windows, Linux e Mac) com um único código. Além disso, ele possui várias baterias incluídas (_batteries included_), que são outros programas (a linguagem chama de _módulo_) que já estão presentes na linguagem, agilizando diversos processos.
 
Um exemplo, é o módulo `os`, que faz referência ao sistema operacional. Ele possibilita fazer diversas tarefas no sistema do computador, como criar pastas ou mover arquivos. É o que o projeto deste artigo precisa. 

    Será feito um programa que recebe um diretório que conteḿ diversos arquivos de imagens, documentos, vídeos, áudios ou outros. O script organizará esses arquivos em suas respectivas pastas. A estratégia será agrupá-los por suas extensões.
 
Assim, a primeira coisa a ser feita é saber o diretório que será organizado.
```python
dir = input("Diretório: ")
```
 
Uma outra forma de fazer isso seria receber a pasta por parâmetro de linha de comando. Isso pode ser feito pelo módulo `sys`. `sys.argv` retorna uma lista com os parâmetros da linha de comando.
 
```python
import sys
 
dir = sys.argv[1]
```
 
Ao executar o programa, o diretório será passado como parâmetro no terminal:
 
```
python3 arquivos.py ~/Imagens
```
 
Com o diretório em mãos, pode-se criar os caminhos para as pastas que serão criadas. `os.path.join()` é responsável por unir o diretório recebido com o nome da pasta. _~/Imagens_ com _Documentos_, por exemplo.
 
A vantagem de usar esse método, é que ele formata o caminho corretamente, independente do sistema operacional. Mac e Linux, por exemplo, utilizam `/` para os caminhos, enquanto Windows `\`. Pode-se alterar a quantidade de pastas ou extensões de acordo com a necessidade. Caso a extensão não se encaixe em uma pasta, ela será movida para `Outros`.
 
```python
documentos = os.path.join(dir, "Documentos")
imagens = os.path.join(dir, "Imagens")
videos = os.path.join(dir, "Vídeos")
audios = os.path.join(dir, "Áudios")
outros = os.path.join(dir, "Outros")
```
 
Agora, é possível criar os diretórios. `os.mkdir()` é o responsável por isso. A condicional `if not os.path.isdir()` verifica se já não existe um diretório com o mesmo nome, pois caso tenha não é necessário criar. Se essa condição não existisse, um erro aconteceria em caso de duplicata de nomes, em uma segunda execução desse programa, por exemplo.
 
```python
if not os.path.isdir(documentos):
  os.mkdir(documentos)
if not os.path.isdir(imagens):
  os.mkdir(imagens)
if not os.path.isdir(videos):
  os.mkdir(videos)
if not os.path.isdir(audios):
  os.mkdir(audios)
if not os.path.isdir(outros):
  os.mkdir(outros)
```
 
Na sequência, é necessário obter a lista dos arquivos ou mesmo pastas no diretório recebido.
 
```python
arquivos = os.listdir(dir)
```
 
A partir disso, vamos percorrer todos e apenas os arquivos (não é de interesse lidar com as pastas), de posse do caminho completo. Também será obtida a extensão de cada arquivo, por meio de `os.path.splitext(caminho)`, que retorna uma lista com o nome do arquivo e sua extensão na segunda posição da lista (índice um). Usa-se o método `lower` para deixar todos os caracteres da extensão em minúsculo.
 
```python
for arquivo in arquivos:
  caminho = os.path.join(dir, arquivo)
  if os.path.isfile(caminho):
       extensao = os.path.splitext(caminho)[1].lower()
```
 
Feito isso, a extensão é comparada com um grupo de extensões em uma lista. Caso a extensão seja `.png`, por exemplo, ela será verificada e definida que deve ser movida para a pasta de imagens. `os.rename` é o responsável por mover.
 
Assim, segue o programa completo:
 
```python
import os
import sys


dir = sys.argv[1]
 
documentos = os.path.join(dir, "Documentos")
imagens = os.path.join(dir, "Imagens")
videos = os.path.join(dir, "Vídeos")
audios = os.path.join(dir, "Áudios")
outros = os.path.join(dir, "Outros")
 
if not os.path.isdir(documentos):
  os.mkdir(documentos)
if not os.path.isdir(imagens):
  os.mkdir(imagens)
if not os.path.isdir(videos):
  os.mkdir(videos)
if not os.path.isdir(audios):
  os.mkdir(audios)
if not os.path.isdir(outros):
  os.mkdir(outros)
 
arquivos = os.listdir(dir)
 
for arquivo in arquivos:
  caminho = os.path.join(dir, arquivo)
  if os.path.isfile(caminho):
      extensao = os.path.splitext(caminho)[1].lower()
      if extensao in [".docx", ".xlsx", ".pptx", ".pdf"]:
          pasta = documentos
      elif extensao in [".jpg", ".jpeg", ".png", ".gif"]:
          pasta = imagens
      elif extensao in [".mp4", ".mkv"]:
          pasta = videos
      elif extensao in [".mp3", ".wma"]:
          pasta = audios
      else:
          pasta = outros
         
      novo = os.path.join(pasta, arquivo)
      os.rename(caminho, novo)
```

Dessa forma, para executar o script, digite em um terminal:
```
python3 nome-script.py caminho-pasta-organizar
```

Exemplo:

```
python3 organiza.py ~/Downloads
```

---
# Referência
Nilo Ney Coutinho Menezes. Introdução à programação com Python: Algoritmos e lógica de programação para iniciantes. Segunda edição. São Paulo: Novatec, 2014.
