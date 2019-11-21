---
layout: post
title: "Controle de Acesso RFID"
categories: ['Automação']
authors: ['João Lucas Fonseca'] 
tags: ['rfid', 'portas']
description: 'Susbstitua suas chaves pela utilização de tags RFID.'
image: rfid.jpg
---


# RFID?

O RFID pode ser definido como uma tecnologia que permite a leitura e gravação de dados entre uma etiqueta (tag) RFID e leitor RFID usando sinais de radiofrequência. Podemos ver o uso de RFID em diversas áreas como por exemplo, identificação de produtos em armazéns, rastreamento de cargas, identificação de animais e até mesmo para armazenamento de dados pessoais.

## COMO FUNCIONA? 

Um sistema de RFID é composto, basicamente, de uma antena, um transceptor, que faz a leitura do sinal e tranfere a informação para um dispositivo leitor, e também um transponder ou etiqueta de rádio frequência, que deverá conter o circuito e a informação a ser transmitida. 

Assim, a antena transmite a informação, emitindo o sinal do circuito integrado para transmitir suas informações para o leitor, que posr sua vez converte as ondas de rádio do RFID para infromações digitais. Agora, depois de convertidas, elas poderão ser lidas e compreendidas por um computador para então ter seus dados analisados

# RFID+Automação Residencial = Praticidade <3

Quem nunca sonhou em deixar sua casa igual a do homem de ferro? Ou pelo menos ter uma persiana que abre após um horário pré determinado, ou quem sabe programar sua cafeteira para fazer café assim que você acordar? Ou simplesmente abrir portas de maneira mais prática, apenas com a aproximação de um cartão, por exemplo. Isso é o que iremos ensinar a você hoje! 

Um dos métodos mais simplificados para realizar tal projeto é a utilização de tags RFID, as quais irão substituir suas chaves e podem ser encontradas em formato de chaveiros, cartões e pulseiras. 


# Abra sua mente (e portas) com o RFID!

Bastante pensado em projetos de automação residencial com Arduino, o esquema para controle de acesso RFID oportuniza a você e a todos os seus familiares ainda maior segurança já que possibilita a abertura de portas de maneira rápida e simples, onde basta passar o cartão em frente ao leitor RFID para liberar a fechadura. Este projeto já é bastante utilizado hoje em dia, e pode ser encontrado em vários hotéis, por exemplo.

Como já dito antes, o sistema de comunicação para transferência de dados do sistema RFID utiliza ondas de rádio, nas quais cada tag emite uma sequência de números como um código exclusivo para cada chaveiro, cartão ou qual for o acessório como, por exemplo, o código do cartão {118, 157, 177, 171, 241} o qual veremos mais a frente na montagem física.

## Produtos Utilizados no Projeto

1. 1 Arduino UNO + Cabo USB AB;
2. 1 Kit RC522 Leitor RFID;
3. 1 Módulo Relé 1 Canal;
4. 1 Display LCD 16×2;
5. 1 Potenciômetro;
6. 1 Fechadura Elétrica 12V;
7. 1 Fonte de Alimentação 12V 1A.

## Montagem Física

Para o perfeito funcionamento do seu Projeto Arduino Controle de Acesso RFID basta seguir de forma rigorosa a pinagem descrita na imagem abaixo, lembrando que alguns cuidados devem ser tomados levando em consideração que diversas são as conexões utilizadas neste projeto.


![rfid](/42/images/post/rfid4.jpg)

## Funcionamento do programa

O funcionamento deste programa é mais simples do que parece. O download do código estará logo abaixo, juntamente com o download das bibliotecas necessárias para o funcionamento do mesmo, copie e cole-os em seu navegador:

**Download do Código:** https://is.gd/036x9i

**Download da Biblioteca:** https://is.gd/J33nWU

### Defina os valores das tags.

Após aplicadas as bibliotecas e com o código aberto, vamos partir para o primeiro passo que é a identificação de nossas tags, a pergunta mais frequente nesta situação é como eu vou fazer para conseguir o valor da minha TAG para incluir no meu projeto? Mas isto é simples, no código disponibilizado acima temos uma variável “int serNum[5];” que é responsável por realizar a leitura de cada tag e através do código, imprimi-la em nosso monitor serial, seja código de acesso aceito ou não, ao aproximarmos o cartão do nosso leitor o que acontece é o seguinte, observe:

![rfid](/42/images/post/rfid5.jpg)

Agora que você já tem a informação do código o qual seu cartão é cadastrado, basta alterar o código existente em seu projeto junto a IDE do Arduino na parte responsável por declarar os códigos liberados para o acesso e compilá-lo novamente, após realizado isto a sua mensagem passará a ser a seguinte:

![rfid](/42/images/post/rfid6.jpg)

Caso deseje adicionar mais de um cartão ao seu projeto, pode o fazer sem problema, porém deve lembrar que os códigos devem seguir sempre o mesmo padrão já existente e que um código deve ser separado de outro inicialmente por uma vírgula e após, um espaço dado pela tecla enter.

# Mandou bem!

Agora que já adicionamos os códigos de cada tag que será liberada a entrar em seu ambiente privado e estamos com o nosso projeto pronto, basta instalá-lo em sua casa ou em seu quarto e mostrar para todo mundo que não é só o Homem de Ferro que possui exclusivas tecnologias de ponta, impressione amigos e familiares com este incrível projeto de automação residencial com Arduino.



