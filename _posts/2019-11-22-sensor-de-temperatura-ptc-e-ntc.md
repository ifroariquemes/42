---
layout: post
title: "Sensores de temperatura: PTC e NTC"
categories: ['Automação']
authors: ['Sabrina Jheniffer'] 
tags: ['Automação','Temperatura','Sensor'.]
description: 'Conheça os sensores de temperatura PTC e NTC'
image: temperatura.jfif
---

Sensor de Temperatura é um componente que sofre variação em uma grandeza elétrica de acordo com uma grandeza física (ex: resistência elétrica x temperatura), desde que exista uma relação conhecida entre a variação elétrica e a grandeza física.

O monitoramento da temperatura por muito tempo limitou-se a ambientes industriais, como por exemplo, no controle de fornos, no monitoramento do funcionamento de máquinas, em controle de processos, entre outros.

A redução do custo dos sistemas automáticos, impulsionada pela disseminação das placas de desenvolvimento de baixo custo e dos conceitos de Internet das Coisas (IoT – Internet of Things), possibilitaram que sensores de grandezas físicas (luminosidade e temperatura) ganhassem importância em ambientes residencias e empresariais.

Hoje, qualquer pessoa pode montar seu próprio sistema de automação que responda sozinho a variações de luminosidade e/ou temperatura utilizando tecnologias baratas tais como placas Arduino.

### Sensor de Temperatura NTC

Os Sensores do tipo NTC possuem resistência inversamente proporcional à temperatura. São mais utilizados por possuírem incrível sensibilidade ao aumento de temperatura e por serem facilmente fabricados. São utilizados para controle, medição ou polarização de circuitos eletrônicos.

O diferencial do NTC é ser muito mais sensível a variações de temperatura, comparado com outros sensores de resistência variável com a temperatura.

São fabricados a partir da mistura de óxidos de metais de transição, manganês, cobre, cobalto e níquel, apresentam variação de resistência ôhmica em relação a temperatura submetida e fabricados a partir de um elemento resistor termicamente sensível que possui um coeficiente negativo.



#### Projetos utilizando sensor de Temperatura NTC:

#### Medindo a temperatura ambiente com Termistor NTC

Serão necessários os seguintes itens:

* 1 x Arduino UNO;
* 1 x Termistor NTC 10k;
* 1 x Resistor 10k;
* 1 x Protoboard;
* Jumpers.

O circuito eletrônico pode ser visto logo abaixo:

![Esquema de montagem do Termistor NTC 10k com Arduino Uno, imagem disponibilizada no site Vida de Silício][/42/images/post/sabrina.jpeg]

#### Resultado prático

![Circuito montado em protoboard, imagem disponibilizada no site Vida de Silício][/42/images/post/sabrina2.jpeg]

![Print screen do monitor serial, disponibilizado no site Vida de Silício][/42/images/post/sabrina3.jpeg]

### Sensor de temperatura PTC:

Os Sensores do tipo PTC possuem resistência proporcional à temperatura, atuam numa faixa restrita em virtude da falta de linearidade e tem como peculiaridade possuírem um ponto de transição, ou seja, somente a partir de uma determinada temperatura exibirá uma variação ôhmica com a variação da temperatura.

A variação da resistência é maior que a de um NTC, na mesma faixa e sua utilização é mais frequente para a medição e proteção térmica de motores e transformadores e máquinas industriais.

Os Sensores PTC são compostos de silício e são ideais para aplicações onde é desejada ótima estabilidade térmica, durabilidade e rápida resposta. Possuem o coeficiente positivo de temperatura de resistência com precisão de 1% a 3% podendo ser utilizado para medições de temperaturas ate 150°C.

![Ecotron Componentes: Sensor de temperatura PTC][/42/images/post/ptc.jpeg]

------------------------------------
Referências:

ADD THERM (Brasil). **CARACTERÍSTICAS DOS SENSORES DE TEMPERATURA NTC E PTC**. 2017. Disponível em: <http://www.addtherm.com.br/sensores-de-temperatura-ntc-e-ptc/>. Acesso em: 22 nov. 2019.

DEMETRAS, Ezequiel. **MEDINDO TEMPERATURA COM TERMISTOR NTC E ARDUINO**. 2019. Disponível em: <https://portal.vidadesilicio.com.br/medindo-temperatura-com-termistor-ntc/>. Acesso em: 22 nov. 2019.

