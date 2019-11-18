---
layout: post
title: "Automação da abertura de portas com Arduino"
categories: ['Automação']
authors: ['Oberdan Martins da Silva Júnior'] 
tags: [Automação, abertura, portas, arduino]
description: 'Construir um prototipo de uma porta ou portão inteligente usando sensor ultrasonico, servo motor e um led. Pode ser aplicado em coisas rotineiras onde é necessário algum tipo de automação em ambientes como casas.'
image: garagem.jpg
---


## Como funciona:

O sensor ultrasonico verifica a distancia de uma pessoa até a porta ou portão, se essa distancia for igual a um determinado valor o servo motor é acionado fazendo com que a porta se abra e logo após liga o led, então espera-se um determinado tempo para que a pessoa possa entrar ou sair do ambiente e novamente é verificado a distancia, caso a distancia seja maior que o valor estipulado o servo motor é acionado novamente fechando a porta e o led (luz) apaga.

# Descrição de cada componente:


## SERVO MOTOR

![Imagem do servo motor](/42/images/post/DESTAQUE.png)

O servo motor ultiliza de  3 fios: um de cor preta, designado para o terra que deve ser ligado ao pino terra do arduino (GND). Um fio vermelho designado para a corrente que deve ser ligado ao pino 5 volts do arduino. E um fio amarelo designado aos dados que deve ser ligado ao pino digital 9 do arduino.

## SENSOR ULTRASONICO

![Imagem do sensor ultrasônico](/42/images/post/imagem-de-destaque-60-1-696x418.png)

O sensor ultrasonico é composto 4 pinos: VCC, Trig, Echo e  GND. O pino VCC deve ser ligado ao pino 5 volt do arduino. O pino Trig deve ser ligado ao pino digital 12 do arduino. O pino Echo deve ser ligado ao pino digital 13 do arduino. O pino GND deve ser ligado ao pino terra do arduino.

## LED

![Imagem do LED](/42/images/post/5mm_Red_LED.jpg)

O led tem dois pinos onde um é maior que o outro. O pino maior, designado para a corrente é ligado a um resistor com o objetivo de regular a tensão que vem do pino digital 10 do arduino. O pino menor (terra) é ligado ao GND (terra) do arduino.

# Código

```c
Servo servo_objeto;
Ultrasonic ultrasonic(12,13);
 
int posicao_inicial_servo = 0;
int ledPin =  10;

void setup()
{
  Serial.begin(9600);
  pinMode(echoPin, INPUT);
  pinMode(trigPin, OUTPUT);
  pinMode(ledPin, OUTPUT);
  servo_objeto.attach(9);
 
}

void loop()
{
   digitalWrite(ledPin, LOW);
   servo_objeto.write(posicao_inicial_servo);
   int valor = func_distancia_ultrasonico();
    if(valor <=15)
    {
        func_controladora();
        delay(5000);
    }
 
  delay(500);
}

void func_controladora()
{
   func_liga_led();
   func_chama_servo();
}

void func_liga_led()
{
  digitalWrite(ledPin, HIGH);
}

void func_chama_servo()
{
  int posicao_final_servo = 90;
  servo_objeto.write(posicao_final_servo);
}

int func_distancia_ultrasonico()
{
  digitalWrite(trigPin, LOW);
  delayMicroseconds(2);
 
  digitalWrite(trigPin, HIGH);
  delayMicroseconds(10);
 
  digitalWrite(trigPin, LOW);
  int distancia = (ultrasonic.Ranging(CM));
  Serial.print("Distancia em CM: ");
  Serial.println(distancia);
  return distancia;
}
```
