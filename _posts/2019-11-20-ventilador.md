---
layout: post
title: "Ventilador 360° com sensor de movimento"
categories: ['Automação']
authors: ['Kristian Da Silva Bernard'] 
tags: [ Direcionamento; Otimização; Gerenciar]
description: 'O projeto visa automatizar um determiando ventilador, para que o mesmo possa direcionar o vento gerado atráves de sensores'
image: vent.jpg 
---

### INTRODUÇÃO 

O projeto desenvolvido tem como objetivo solucionar o problema que é o direcionamento do vento do ventilador e o gasto desnecessário de energia. Ao implantar este projeto será possível promover uma baixa no gasto energético levando em conta que ao não detectar movimento o ventilador desligará automaticamente, considerando que o mesmo vai girar 360°, havendo também uma grande otimização no desempenho do mesmo, já que ele poderá rotacionar para qualquer ponto ao detectar movimento. Isso se dará através de sensores de movimentos ligados a um Arduino e ao ventilador, que será capaz de gerenciar os sensores através de um código fonte. 

### METODOLOGIA

No presente projeto foi utilizada a ferramenta de desenvolvimento de circuitos e desenhos 3D
denominada Tinkercad, ao qual foi desenvolvido um circuito utilizando o Arduino uma plataforma de prototipagem eletrônica de hardware livre e de placa única. Para a detecção do movimento humano foram utilizados alguns sensores PIR(Passive Infrared Sensor - Sensor Infravermelho Passivo) aos quais foram ligados ao Arduino que executa o código fazendo a função de controlador.

### RESULTADOS E DISCUSSÕES

A Figura 1, apresenta o modelo conceitual do projeto do Ventilador com sensor de 
Movimentos. Para fazer o mesmo precisamos de 1 placa de Arduino UNO; 1 placa de ensaio pequena, 1 palca de ensaio mini; 1 capacitor de 100µF; 5 LED’s; 5 Sensores de Movimento PIR; 5 resistores de 220 ohm e 2 Servos Motores (Tower Pro MG996R), como na Ferramenta Tinkercad só serve para montar 
circuitos, não é possível adicionar componente como Ventiladores. A Figura 2, apresenta parte 
do código necessário para o funcionamento do projeto.

![Modelo conceitual](/42/images/thumbs/arduino.png)
![Código de Programação](/42/images/thumbs/codigo.png)
