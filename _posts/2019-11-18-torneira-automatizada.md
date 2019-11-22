---
layout: post
title: "Torneira Automatizada"
categories: ['Automação']
authors: ['Karina Gois Almeida'] 
tags: ['consumo','automatizada','torneira']
description: 'Projeto para economia de água com uma torneira automatizada'
image: agua011.jpg
---

Muitas coisas influenciam no consumo de água. Por exemplo lavar uma louça ou até mesmo a mão, quando vai lavar louça exige um alto consumo de água, assim gerando um 
grande desperdício de água e prejudicando o meio ambiente. Mas com o avanço de estudos tiveram a ideia de fazer uma torneira automatizada, o intuito dela e fazer
um bom aproveito da água sem muito consumo. E essa torneira seria de grande ajuda nas escolas, por exemplo.

Neste artigo vou mostrar um tutorial de torneira automatizada sem muito gastos. Para ser feita essa torneira iremos precisar dos seguintes componentes:

- Fotorresistor;
- Arduino Uno R3
- Blackboard pro mini 5v/16MHz;
- 1 kΩ Resistor;
- 180 Ω Resistor;
- LED RGB.

O funcionamento é simples. O Micro servo ele vai realizar  o trabalho de uma válvula que iŕa bloquear e liberar a passagem de água.Então para deixar esse equipamento possível para colocar em qualquer ambiente, reduzimos ele usando a placa (Blackboard pro mini 5V/16MHz tendo a mesma funcionalidade dada Blackboard convencional porém em um tamanho reduzido, para fazermos esse procedimento devemos primeiro fazer um protótipo em uma placa blackboard no tamanho convencional.Então conforme o objeto estiver chegando perto do fotorresistor ele irá acionar e passará comandos para o micro servo que irá liberar uma quantidade de água, então se o objeto chegar  mais perto do sensor ela vai entender que precisa energizar, se o objeto estiver mais distante ela para de energizar, diminuindo o fluxo de água. O código é muito simples, vai fazer uma leitura do pino analógico e conforme for o valor lido vai desacionar e acionar. Assim se tudo estiver Ok passaremos para o teste real.

## Código fonte do programa que executará na torneira

```c
#include <Servo.h>
Servo s; // Variável Servo
 void setup()
{
  pinMode(2, OUTPUT);
  pinMode(3, OUTPUT);
  Serial.begin(9600);
  s.attach(4);
  s.write(0); 
}

void loop()
{
  int leitura = analogRead(A0);
  if(leitura>400){
  	digitalWrite(3, HIGH);
    digitalWrite(2, LOW);
  	s.write(90); 
  }else {
  	digitalWrite(2, HIGH);
    digitalWrite(3, LOW);
  	s.write(0); 
  }
}
```
!["Projeto tinkercad"](/42/images/post/foto.png)


### Referências  
[https://www.tinkercad.com/things/2bZ0meLgIDR-torneira-automatica](https://www.tinkercad.com/things/2bZ0meLgIDR-torneira-automatica)
[https://www.robocore.net/tutoriais/fazendo-uma-torneira-automatica-com-arduino](https://www.robocore.net/tutoriais/fazendo-uma-torneira-automatica-com-arduino)

