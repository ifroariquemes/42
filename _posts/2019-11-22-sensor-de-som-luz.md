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

 - 1 Sensor de som KY-038
 - 1 Relé de estado sólido 
 - 1 Lâmpada (ou qualquer outro objeto que se deseja acionar)
 - 1 Arduino Uno

*OBS.:* Tome cuidado ao escolher o relé, pois os mesmos, são feitos para corrente alternada (AC) não funcionam para corrente contínua (DC). Para este caso, como iremos utilizar uma carga de AC este relé escolhido é apropriado. 

#### Montagem do circuito 

Como estamos utilizando a saída digital do Sensor de som KY-038, vamos utilizar uma entrada digital do Arduino. Apesar de utilizarmos um Arduino Uno no exemplo, poderia ser qualquer outra placa de desenvolvimento.

![circuito conceitual](/42/images/thumbs/circuito.png)

Para que o nosso circuito possa ser acionado atráves do estalo das palmas, precisamos de um código de programação. 

```c
//Programa para acender as luzes com palmas
int pino_som = 7; //Define o pino que será utilizado para o sensor de som
int pino_rele = 5;     //E o que será utilizado para o rele
boolean rele = HIGH; // Define um booleano para poder usar a operacao NAO

void setup() {
  pinMode(pino_som, INPUT); //Coloca o pino do sensor de som como entrada
  pinMode(pino_rele, OUTPUT);   // E o do rele como saida
}

void loop() {
  int som = digitalRead(pino_som); //Verifica se a saida do sensor esta ativa
  
   if(som){ // Se o som estiver alto
    rele = !rele; //Operacao NAO: Se estiver LOW, passa pra HIGH. Se estiver HIGH passa para LOW
    digitalWrite(pino_rele, rele); // Manda o valor da variavel para o rele
    delay(1000); // Aguarda 1 segundo para não ficar ligando e desligando sem parar
   }
}
```

### Conclusão 

Podemos perceber que com a automatização de acender uma lâmpada de modo tradiconal, teremos uma praticiade ao mudar esse "tradiconal" por algo mais inovador.


Referências: [https://www.filipeflop.com/blog/sensor-de-som-acender-luz-palmas/](https://www.filipeflop.com/blog/sensor-de-som-acender-luz-palmas/)


