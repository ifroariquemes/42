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

A sigla RFID significa Radio Frequency Identification ou Identificação por Radiofrequência. Ciriaco (2009), define o RFID da seguinte maneira:

> Uma tecnologia que permite a leitura e gravação de dados entre uma etiqueta (tag) RFID e leitor RFID usando sinais de radiofrequência."

Podemos ver o uso de RFID em diversas áreas como por exemplo, identificação de produtos em armazéns, rastreamento de cargas, identificação de animais e até mesmo para armazenamento de dados pessoais.

## COMO FUNCIONA? 

Um sistema de RFID é composto, basicamente, de uma antena, um transceptor, que faz a leitura do sinal e transfere a informação para um dispositivo leitor, e também um transponder ou etiqueta de rádio frequência, que deverá conter o circuito e a informação a ser transmitida. 

Assim, a antena transmite a informação, emitindo o sinal do circuito integrado para transmitir suas informações para o leitor, que por sua vez converte as ondas de rádio do RFID para infromações digitais. Agora, depois de convertidas, elas poderão ser lidas e compreendidas por um computador para então ter seus dados analisados.

A aplicação do RFID é muito ampla, podendo ajudar em várias coisas no cotidiano, como no rastreamento animal, identificação de alguma objeto que você perde frequentemente (controle da televisão), etc. Dessa forma, mostra-se evidente a importancia do RFID, haja vista a grande praticidade e facilidade ofertadas. 

## RFID+Automação Residencial = Praticidade <3

Quem nunca sonhou em deixar sua casa igual a do homem de ferro? Ou pelo menos ter uma persiana que abre após um horário pré determinado, ou quem sabe programar sua cafeteira para fazer café assim que você acordar? Ou simplesmente abrir portas de maneira mais prática, apenas com a aproximação de um cartão, por exemplo. Isso é o que iremos ensinar a você hoje! 

A melhor maneira de realizar esse projeto é com as tags RFID. Espera, você não sabe o que é? Então conheça um pouco mais sobre o assunto abaixo!

## O que é Tag RFID e sua aplicação no Arduino

A grosso modo, podemos dizer que os marcadores de RFID são os novos códigos de barra já que, assim como eles, essas tags permitem que a leitura das informações seja feita automaticamente por sensores, sem a necessidade de aproximar o código ao leitor. Hoje em dia, essas tags estão presentes em quase todo canto.

O leitor RFID tem 8 pinos. Para o funcionamento da aplicação das tags com o arduino é necessário utilizar o seguinte sistema elétrico:

![sistema elétrico](/42/images/post/arduino.jpg)
Fonte: canal Vixe Effets (2015) 

* Pino SDA ligado na porta 10 do Arduino
* Pino SCK ligado na porta 13 do Arduino
* Pino MOSI ligado na porta 11 do Arduino
* Pino MISO ligado na porta 12 do Arduino
* Pino NC – Não conectado
* Pino GND ligado no pino GND do Arduino
* Pino RST ligado na porta 9 do Arduino
* Pino 3.3 – ligado ao pino 3.3 V do Arduino

Feito isso, sempre que aproximar o marcador RFID do arduino será imprimida uma mensagem no leitor serial com o número do identificador.

# Abra sua mente (e portas) com o RFID!

O seguinte projeto foi desenvolvido pelo blog **Usina Info**, e publicado por Matheus Straug, que o apresenta dizendo:

> Bastante pensado em projetos de automação residencial com Arduino, o esquema para controle de acesso RFID oportuniza a você e a todos os seus familiares ainda maior segurança já que possibilita a abertura de portas de maneira rápida e simples, onde basta passar o cartão em frente ao leitor RFID para liberar a fechadura." Straug (2017)

Straug da continuidade dizendo que o sistema de comunicação para transferência de dados do sistema RFID utiliza ondas de rádio, nas quais cada tag emite uma sequência de números como um código exclusivo para cada chaveiro, cartão ou qual for o acessório como, por exemplo, o código do cartão {118, 157, 177, 171, 241} o qual veremos mais a frente na montagem física.


## Montagem Física

Para o perfeito funcionamento do seu Projeto Arduino Controle de Acesso RFID basta seguir de forma rigorosa a pinagem descrita na imagem abaixo, lembrando que alguns cuidados devem ser tomados levando em consideração que diversas são as conexões utilizadas neste projeto.


![rfid](/42/images/post/rfid4.jpg)
Fonte: Straub, Matheus. Usina Info (2017)

## Funcionamento do programa

O funcionamento deste programa é mais simples do que parece. O download do código estará logo abaixo, juntamente com o download das bibliotecas necessárias para o funcionamento do mesmo, copie e cole-os em seu navegador:

**Download do Código:** https://is.gd/036x9i
     Fonte: Straub, Matheus. Usina Info (2017)

**Download da Biblioteca:** https://is.gd/J33nWU
     Fonte: Straub, Matheus. Usina Info (2017)

Finalizado o download, abra o código e aplique as bibliotecas para poder seguir pro próximo passo: 

## Defina os valores das tags.

Como? É muito simples, no código disponibilizado acima contém uma variável “int serNum[5];”. Essa variável será a responsável por realiar a leitura de cada tag e através do código, imprimi-la no monitor serial, seja código de acesso aceito ou não. Feito

![rfid](/42/images/post/rfid5.jpg)
Fonte: Straub, Matheus. Usina Info (2017)

Agora que você já tem a informação do código o qual seu cartão é cadastrado, basta alterar o código existente em seu projeto junto a IDE do Arduino na parte responsável por declarar os códigos liberados para o acesso e compilá-lo novamente, após realizado isto a sua mensagem passará a ser a seguinte:

![rfid](/42/images/post/rfid6.jpg)
Fonte: Straub, Matheus. Usina Info (2017)

Caso deseje adicionar mais de um cartão ao seu projeto, pode o fazer sem problema, porém deve lembrar que os códigos devem seguir sempre o mesmo padrão já existente e que um código deve ser separado de outro inicialmente por uma vírgula e após, um espaço dado pela tecla enter.

# Mandou bem!

Agora que já adicionamos os códigos de cada tag que será liberada a entrar em seu ambiente privado e estamos com o nosso projeto pronto, basta instalá-lo em sua casa ou em seu quarto e mostrar para todo mundo que não é só o Homem de Ferro que possui exclusivas tecnologias de ponta, impressione amigos e familiares com este incrível projeto de automação residencial com Arduino.


# REFERÊNCIAS

Ciriaco, Douglas. Como funciona a RFID?. **TECMUNDO**, 2009. Disponível em: <https://www.tecmundo.com.br/tendencias/2601-como-funciona-a-rfid-.htm>. Acesso em: 19 de novembro de 2019.

Straub, Matheus. Automação Residencial RFID. **USINA INFO**, 2007. Disponível em <https://www.usinainfo.com.br/blog/projeto-arduino-controle-de-acesso-rfid/>. Acesso em: 19 de novembro de 2019

Silveira, Geovana. O que é a tecnologia RFID e como ela pode ajudar sua empresa?. **RFID BRASIL**, 2017. Disponível em: <https://rfidbrasil.com/blog/o-que-e-a-tecnologia-rfid-e-como-ela-pode-ajudar-sua-empresa/>. Acesso em: 21 de novembro de 2019


