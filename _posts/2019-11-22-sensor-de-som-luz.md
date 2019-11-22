---
layout: post
title: "Acendendo uma Lâmpada com Sensor de Som"
categories: ['Automação']
authors: ['Welignton Campanari'] 
tags: []
description: 'Esse projeto visa a praticidade para acender uma lâmpada de um determinado ambiente, através de um sensor de som'
image: lamp.jpg
---
### Introdução

Seria muito mais prático usar sons para acender e desligar luz. Por exemplo quando você já está longe do interruptor e tem preguiça de levantar novamente para apagar a luz ou está com muita pressa para sair e o interruptor fica longe. 

### Desenvolvimento

#### Materiais para a produção do circuito 

 > 1 Sensor de som KY-038
 > 1 Relé de estado sólido 
 > 1 Lâmpada (ou qualquer outro objeto que se deseja acionar)
 > 1 Arduino Uno

*OBS.:* Tome cuidado ao escolher o relé, pois os mesmos, são feitos para corrente alternada (AC) não funcionam para corrente contínua (DC). Para este caso, como iremos utilizar uma carga de AC este relé escolhido é apropriado. 

#### Montagem do circuito 

Como estamos utilizando a saída digital do Sensor de som KY-038, vamos utilizar uma entrada digital do Arduino. Apesar de utilizarmos um Arduino Uno no exemplo, poderia ser qualquer outra placa de desenvolvimento.
!["circuito conceitual"] (/home/kristian/42/images/thumbs/circuito.png)
Para que o nosso circuito possa ser acionado atráves do estalo das palmas, precisamos de um código de programação. 
!["código de programação"] (/home/kristian/42/images/thumbs/programacao.png)

### Conclusão 

Podemos perceber que com a automatização de acender uma lâmpada de modo tradiconal, teremos uma praticiade ao mudar esse "tradiconal" por algo mais inovador.


Referências: [https://www.filipeflop.com/blog/sensor-de-som-acender-luz-palmas/](https://www.filipeflop.com/blog/sensor-de-som-acender-luz-palmas/)


