---
layout: post
title: "Sensor ultrassônico - Funcionamento e aplicação"
categories: ['Automação']
authors: ['Iago Macedo'] 
tags: [sensores, distância]
description: 'Conceituação e aplicação de sensores capazes de medir a distância utilizando ondas ultrassônicas'
image: iago3.jpg
---


 Os sensores são baseados em duas principais partes para que o seu funcionamento seja realizado. O primeiro deles é o emissor, que tem como propriedade exclusiva a de emitir uma onda de alta frequência (Cerca de 40khz), esta onda emitida segue até o objeto mais próximo, ao colidir com o objeto a onda é refletida e retorna ao sensor ativando o receptor. Este dispositivo é capaz de identificar as ondas que, anteriormente foi lançada pelo emissor, e através de uma expressão matemática definir a distância entre o sensor e o objeto. Esta expressão só é possível pelo fato da velocidade do som no ar já ser conhecida (340 m/s), tendo isso em vista, no momento em que a onda é emitida um relógio de alta precisão cronometra o intervalo de tempo que a onda leva para ir e voltar tornando possível o cálculo da distância.


### Fórmula do sensor 

A fórmula utilizada pelo sensor se dá pela seguinte expressão: d = (V*t)/2

- d = distância entre o sensor e o obstáculo 
- V = velocidade do som no ar (340 m/s), é uma constante
- t = tempo percorrido entre a emissão do sinal sonoro e o seu retorno
- A divisão por 2 dá-se devido ao fato do sensor considerar o tempo de ida e volta, ou seja, duas vezes o tempo almejado.


Imagem para instigar e melhorar a identificação do processo de funcionamento do sensor:
![image](/42/images/post/iago.jpg)
 
## Aplicação

 Os sensores de cunho ultrassônico vem ganhando espaço no âmbito comercial devido a acessibilidade que ele proporciona nos diversos desafios do dia a dia, nos projetos, principalmente da automação e aqueles que são aplicados em grandes indústrias, considerando que ele pode  ser utilizado na medição de distâncias e níveis sem contato, na contagem de objetos transparente, entre outros.

Depois de passar sobre um breve conceito sobre os sensores ultrassônicos, é possível desenvolver uma básica aplicação inetegrada ao arduino

Material a ser usado:

- 01x Arduino Uno R3 Compatível + Cabo Usb
- 01x Sensor de Distância Ultrassônico HC-SR04
- 1x Protoboard 400 Pontos
- 4x Jumpers MxM

![image](/42/images/post/iago1.jpg)

### O código 

```c

 #include < Ultrasonic.h > 
 #define trigger  5 
 #define echo 6
 
 Ultrasonic ultrasonic(trigger, echo);
  void setup()
 {
  Serial.begin(9600);
  Serial.println("lendo os dados.."); 
  }
 
 void loop()
 {

    float cmMsec;
    long microsec = ultrasonic.timing();
    cmMsec = ultrasonic.convert(microsec, Ultrasonic::CM);
    Serial.print("Distância: ");
    Serial.print(cmMsec);
    delay(500);

}

```
 



### Resultado

Os dados deverão ser exibidos no monitor serial, estes dados correspondem a distância entre o sensor e o objeto. O site Tinkercad e o site fritzing, ambos sites de manipulação de projetos tecnológicos, são ótimos para fazerem testes antes de criarem o projeto físico. 





## Conclusão

O sensor mais recomendado é o HC-SR04, um sensor que lhe permite várias aplicações, sua programação é simples, possui muitas explicações na internet, o que faz dele o sensor mais comum no mundo tecnológico. Com mais alguns ajustes o projeto poderia ser aplicado a um projeto maior de maior eficiência. Mas para fazer isso seria necessário diversas novas configurações. Porém, caso feito, o projeto poderia atender várias necessidades, sendo elas de grande relevância ou não, e é o que torna ainda mais interessante a aplicação desse projeto. É realmente desafiador, exige-se muito tempo e esforço, mas é válido o conhecimento.


# Referências 

CircuitsToday.  (2013).  CircuitsToday.  Acesso  em  Novembro  de  2019,  disponível  em  [http://www.circuitstoday.com/ultrasonic-range-finder-using-8051](http://www.circuitstoday.com/ultrasonic-range-finder-using-8051).

NAKATANI, Alessandro Massayuki; GUIMARÃES, Anderson Valenga; NETO, Vicente Machado. MEDIÇÃO COM SENSOR ULTRASSÔNICO HC-SR04. In: NAKATANI, Alessandro Massayuki; GUIMARÃES, Anderson Valenga; NETO, Vicente Machado. MEDIÇÃO COM SENSOR ULTRASSÔNICO HC-SR04. 2013. Tese (Superior) - UTFPR, [S. l.], 2013. Disponível em: [http://www.energiapura.net.br/Trabalhos%20Publicados/2014/sensor_ultrassom_arduino_cimmec_2014.pdf](http://www.energiapura.net.br/Trabalhos%20Publicados/2014/sensor_ultrassom_arduino_cimmec_2014.pdf). Acesso em: 19 nov. 2019.

Ultrasonic  Ranging  Module  HC-SR04.  Elecfreaks. Datasheet.  Disponível em:[http://users.ece.utexas.edu/~valvano/Datasheets/HCSR04b.pdf](http://users.ece.utexas.edu/~valvano/Datasheets/HCSR04b.pdf) Acessado em 19 Nov. 2019. 





















 



