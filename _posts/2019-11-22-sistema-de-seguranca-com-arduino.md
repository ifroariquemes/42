---
layout: post
title: "Sistema de segurança com arduino"
categories: ['Automação']
authors: ['Elizeu Batiliere'] 
tags: ['Automação','Residência','Segurança'.]
description: 'Post para apresentar alguns projetos que objetivam a construção de um sistema de segurança com arduino'
image: seguranca.png
---

## Sistema de segurança residencial com arduino##

Quando falamos de segurança, falamos também de tecnologia. A segurança está em pauta, principalmente no Brasil. Mesmo que assegurada pela Declaração Universal dos Direitos Humanos, o direito básico de segurança pública de qualidade ainda não é praticado no Brasil.

Procurando inverter isso, desenvolvedores estão construindo soluções para transformar residências e empresas mais seguras com câmeras, portas inteligentes, alarmes, sensores e até dispositivos de laser.

Em uma maquete, o pessoal do canal [Jun Peng](https://www.youtube.com/channel/UCZj3U-ojTNasP2sTQyw1y9g) desenvolveu um projeto complexo de segurança residencial.

No vídeo, ele realizou a montagem para demonstração. O canal também disponibilizou os arquivos para desenvolver o projeto, seja em ‘modo’ mini ou real.

### Sistema de fechadura inteligente

Para este sistema funcionar, pode-se configurar uma sequência de batidas na porta, adicionar senha ou biometria. Embora o projeto cause dúvidas em relação à segurança, podemos garantir sua funcionalidade, haja vista que, para que alguém consiga descobrir a combinação exata das batidas na porta, seria necessário que essa pessoa vigiasse o morador, afim de causar algum transtorno ou praticar um crime, uma vez que os toques são necessários para abrir a porta. 
No vídeo, cedido por Leonardo Loiacono em um sistema projetado por ele mesmo, vemos um sistema bastante útil, que não necessita de senhas, ou biometria, mas sim o popular “Toc-Toc-Toc”. Acesse: <https://youtu.be/wZ9oFYFTaqM>.

### Alarme com Arduino e sensor de movimentos PIR.

ste projeto de alarme é capaz de detectar movimentos em um ambiente disparando um sinal sonoro e acendendo um led. Pode ser usado por exemplo na porta de entrada da sua casa ou em algum cômodo e quando alguém passar por lá o alarme será disparado. Então se você necessita ser avisado da presença de alguém em um determinado lugar este projeto é uma opção interessante e fácil de fazer.

O sensor PIR é fácil de se encontrar, a maioria das lojas virtuais e físicas que vendem Arduinos e/ou componentes eletrônicos normalmente possuem este sensor. Só verifique se o sensor PIR que você pretende adquirir possui controle de sensibilidade da detecção de movimentos. Este que usei no projeto do alarme possui três pinos, controle de sensibilidade e controle de tempo que o sensor fica "ligado" quando detecta algum movimento.

Para desenvolver o projeto Alarme com Arduino e sensor de movimentos PIR você vai precisar de:

* Arduino;
* sensor de movimentos/presença PIR;
* led;
* buzzer de 5 volts;
* 2 resistores de 220 ohms;
* protoboard;
* bateria de 9 volts;
* suporte para bateria com plug para ligar no Arduino;
* fios para interligar os componentes.

Segue abaixo o esquema detalhado do projeto do Alarme com Arduino e sensor de movimento PIR. Através deste esquema fica mais fácil de se ter uma visão geral, e de como montar corretamente o projeto. Este esquema foi montado no software Fritzing.

![Circuito para o projeto de alarme com arduino][/42/images/post/alarme.jpg]

Para ver o código, acesse: <http://www.comofazerascoisas.com.br/como-fazer-um-alarme-com-arduino-sensor-de-movimentos-pir.html>

Para ver o projeto em funcionamento acesse: <https://youtu.be/gHMe-YhL_oc>

### Sistema de segurança utilizando Lasers:

O site [Fisici Senza Palestra](https://www.fisicisenzapalestra.com/) criou um sistema bastante simples, e que pode ser utilizado para pegar qualquer intruso que queira invadir sua residência.

O laser serve apenas como sensor, possível de identificar quaisquer movimento em no ambiente em que foi instalado. Ah! Nada de lasers cortantes, como nos filmes de ação, hein!?

Para a realização do projeto, você vai precisar de poucos componentes, como dois LEDs, um Speaker, um botão pulsante, um Laser e um Fotoresistor.

Caso tenha interesse no projeto, você pode clicar neste [link](http://www.fisicisenzapalestra.com/tecnologicamente/arduino/allarme-laser-arduino/) e seguir o tutorial em italiano.

### Sistema Anti-roubo GSM

A Electros Chematics desenvolveu um sistema bastante simples e que envia SMS para o usuário quando seus sensores de presença são acionados. Isso já funciona com dispositivos e equipamentos da Intelbras e de outras fabricantes de alarmes e sistemas de proteção residencial. No entanto, é válido ressaltar que esse é um projeto caseiro, e pode ser útil para quem quer economizar.

----------------------------------------
Referências:

COMO FAZER AS COISAS (Brasil). **Como fazer um Alarme com Arduino e sensor de movimentos PIR**. Disponível em: <http://www.comofazerascoisas.com.br/como-fazer-um-alarme-com-arduino-sensor-de-movimentos-pir.html>. Acesso em: 22 nov. 2019.

VICTOR, Felipe. **Projetos incríveis de segurança feitos com Arduino**. 2016. Disponível em: <https://www.tecstudio.com.br/tecnologia/projetos-incriveis-de-seguranca-feitos-com-arduino/>. Acesso em: 22 nov. 2019.
