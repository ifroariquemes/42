---
layout: post
title: "projeto com arduino para irrigação automática de jardins"
categories: ['Automação']
authors: ['Lucas De Moura Rodrigues'] 
tags: [Projeto, arduino, irrigação e jardim]
description: 'Neste projeto vou mostrar pra vocês um sistema de irrigação feito inteiramente em casa, utilizando Arduíno, alguns módulos e materiais que podem ser encontrados em qualquer deposito de construção.'
image: lucass.jpg
---

#Sistema de Irrigação com Arduino

Para fazer o sistema de irrigação com arduino, utilizaremos uma válvula solenoide de entrada de água, modelo VA05-12V. Ela funciona com uma tensão de 12V DC, possui rosca de 3/4″ e a pressão de operação é de 0,2 à 8 kgf/cm². Com a pressão de 0,2 kgf/cm² a vazão chega a 7 litros/min. Já a 8 kgf/cm² pode chegar a 40 litros/min.

!["imagem válvula"](/42/imagens/_post/valvula.jpg)

Pode ser utilizada em sistemas de irrigação, abastecimento e muitas outras aplicações. O fluido utilizado (água, etc.) deve ter a temperatura até 60ºC.

#Materiais Necessários

    1 Unidade – Arduino Uno
    1 Unidade – Sensor de umidade de solo
    1 Unidade – Módulo Relé 5V
    1 Unidade – Jumper Macho Macho
    1 Unidade – Jumper Macho Fêmea
    1 Unidade – Válvula solenoide para água 12V VA 05
    1 Unidade – Fonte 12V/1A
    1 Unidade – Adaptador P4 fêmea
    1 Unidade – Mangueira
    1 Unidade – Terminal Faston fêmea (opcional)
    1 Unidade – Ferro de Solda e Estanho (opcional)
    1 Unidade – Vaso com planta


#Circuito em Fritzing

A seguir temos o esquemático em Fritzing para o projeto irrigação com arduino:

!["imagem válvula"](/42/imagens/_post/lucas.jpg)

Utilizamos uma fonte 12V conectada ao adaptador p4 para alimentar o Arduino e a válvula. O relé fará o chaveamento da tensão para ligar/desligar a válvula.

Os conectores da válvula possuem entrada do tipo Faston 6,3mm x 0,8mm fêmea. Caso não tenha estes conectores, solde dois fios nestes terminais para utilização.

Verifique se o relé é ativado em nível LOW (0V) ou HIGH (5V). Para este projeto, utilizamos um relé que fecha o contato em nível LOW.

Os relés possuem três contatos: NO (ou NA – normalmente aberto), comum (COM) e NC (ou NF – normalmente fechado). As conexões foram realizadas nos contatos NO e COM, ou seja, o contato do relé fecha e ativa a válvula. Caso queira que a válvula se mantenha sempre aberta e feche quando atingir certa condição, serão usados os contatos NC e COM. Não utilize NO e NC sem o contato COM, pois não funcionará corretamente.


#Programação

A seguri o código:

'''c
int valvula = 8; // sinal do rele para válvula
 
void setup() {
  pinMode(valvula, OUTPUT); // declara válvula como saída
}
 
void loop() {
 
 // Leitura do sensor no pino A0 e armazenamento em SensorValue
 
 int sensorValue = analogRead(A0);
 
 // verifica se valor de leitura está acima de 600 (umido abaixo de 600  e seco até 1023)
 
 if (sensorValue > 600){
   // se sim, libera água por 1s
   digitalWrite(valvula,LOW);
   delay(1000);
   digitalWrite(valvula,HIGH); // desliga válvula
 }
 
 else{
 // se não, interrompe a passagem de água
   digitalWrite(valvula,HIGH);
   delay(1000);
  }
  delay(3000); // Aguarda 3s para verificar se solo está umido novamente
}
'''c


Se você desejar que o relé fique ativado por mais ou menos tempo, mude o valor dos delay nos comandos IF e ELSE.


