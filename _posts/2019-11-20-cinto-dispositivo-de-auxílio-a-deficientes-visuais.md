---
layout: post
title: "Cinto: Dispositivo de auxílio a deficientes visuais"
categories: ['Automação']
authors: ['Jocássia Dolci'] 
tags: ['acessibilidade','automação','cinto']
description: 'O presente post, visa apresentar o cinto que auxília deficientes visuais, projeto desenvolvido pela escola Nossa Senhora de Fátima'
image: def.jpg
---

A motivação encontrada para efetuar o trabalho proposto está ligada a auxiliar os deficientes visuais a fim de proporcionar experiência provavelmente inalcançável devido ao fato de possuírem esse problema, baseando-se em um projeto que venha a ter um baixo custo e uma boa eficiência, a fim de alcançar o objetivo referente ao trabalho. Este trabalho teve como principal norteador a possibilidade de utilizar ondas sonoras para dar noção de campo sensitivo e identificação de diversos tipos de objetos. Baseando-nos nessa hipótese, procuramos auxiliar pessoas com diversos problemas, assim foi decidido utilizar essa tecnologia para ajudar deficientes visuais na percepção do espaço. Porém, para utilizar essa tecnologia de uma maneira simples e adaptável a qualquer situação, é proposta a forma de um cinto que se ajusta de acordo como o corpo do usuário. O trabalho foi construído utilizando objetos simples de fácil acesso no mercado e sensores ultrassônicos controlados por meio de uma plataforma livre. O projeto foi desenvolvido na instituição de ensino utilizando-se dos materiais de fácil acesso, de preferência reutilizados, sendo também aplicados conhecimentos sobre eletrônica, programação, mecânica e 
física.

MATERIAIS:

Para a produção do dispositivo, foram utilizados diversos materiais, dentre os quais incluem:

• microcontrolador;
• sensores ultrassônicos;
• motores de vibração;
• bateria;
• placa de circuitos;
• materiais para confecção da base do cinto.

Construção:

Inicialmente foram feitos orifícios em um elástico preto, utilizado como tecido e base do cinturão, para a disposição dos sensores ultrassônicos. Em seguida, os motores de vibração foram fixados logo abaixo dos sensores ultrassônicos utilizando cola aquecida. Consecutivamente, todos os componentes foram ligados a fios que, posteriormente, foram ligados ao microcontrolador.

Para sua correta utilização, o dispositivo deve estar posicionado na cintura do deficiente visual, com os sensores ultrassônicos direcionados à sua frente.

FUNCIONAMENTO:

Foi elaborado um algoritmo que analisa a distância encontrada pelos sensores ultrassônicos para checar a relação entre o espaço disponível para locomoção. Caso perceba-se que esse espaço está diminuindo, significando que existe algum obstáculo à frente, os motores de vibração começarão a funcionar, fornecendo um retorno tátil para o deficiente.

Para que haja uma maior precisão no retorno tátil direcionado ao deficiente, a potência aplicada nos motores de vibração será inversamente proporcional à distância encontrada pelos sensores ultrassônicos, ou seja, quanto mais longe, mais fraco será o retorno tátil (tendo sido previamente configurado para que o retorno tátil seja 0% com valores acima de 2 metros, sendo possível a mudança desse valor), e quanto mais perto, mais forte e perceptível será o retorno tátil. Para criar uma maior segurança para o deficiente visual, caso os sensores ultrassônicos achem uma distância menor que 20 centímetros, além do retorno tátil, serão executados vários bips, fornecendo um retorno auditivo.

CONCLUSÕES:

Ao final de exaustivos testes, o dispositivo apresenta um bom funcionamento, exceto por falhas mínimas, que não interferem no propósito principal do dispositivo. Com a tentativa de resolução desses problemas, o dispositivo se mostrou bastante eficaz em auxiliar pessoas que, após a visão bloqueada para simularem a condição de um deficiente visual, se viram em um labirinto com diversos obstáculos para o teste do dispositivo.


_________________________________________________________________________

REFERÊNCIAS:

CARVALHO, Ítalo Lélis de et al. CINTO: DISPOSITIVO DE AUXÍLIO A DEFICIENTES VISUAIS. 2013. Disponível em: <https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=2ahUKEwiAqMGL1_nlAhVNHLkGHcgEBK4QFjAAegQIARAC&url=http%3A%2F%2Fsistemaolimpo.org%2Fmidias%2Fuploads%2F12a54f961eb531d15e915497a262ae28.pdf&usg=AOvVaw3wX-tW0O4yg6qeLvYFTAlu>. Acesso em: 20 nov. 2019.
