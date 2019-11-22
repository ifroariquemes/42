---
layout: post
title: "Aplicações do servo motor em projetos de automação"
categories: ['Automação']
authors: ['Matheus Siqueira'] 
tags: [Servo Motor, Servo Motor CA, Servo Motor CC, Servo Motor de Passo]
description: Post sobre o funcionamento de um servo motor e as diferentes formas de encapsulamento, agrupados por faixa de torque. Demonstrar aplicações em que eles se aplicam.
image: Servo.jpg
---

O Servomotor é uma máquina eletromecânica, que demonstra um movimento proporcional a um comando desejado, logo o mesmo é um atuador rotativo ou linear que garante o controle, velocidade e precisão em aplicações de controle de posição em malha fechada.

### Servo Motor CA

Os servo motores são classificados em CA (corrente alternada) e CC (corrente contínua). Os servo motores CC são empregados em projetos menores devido ao seu custo, simplicidade e eficiência. Os Servo motores CA são mais frequentemente utilizados na indústria por suportar tarefas que utilizam mais potência e fornece exatidão superior na hora de controlar e taxa de manutenção baixa.

Os servos CA são normalmente divididos em 2 categorias, sendo elas os síncronos e os de indução. Temos ainda um terceiro tipo que por sua vez é mais empregado em aplicações menores que seria o motor de passo.

![TABELA SERVO MOTOR](/42/images/post/TABELA SERVO MOTOR.JPG)

### Servo Motor de Passo

Os tipos de servi motores de passo podem ser o Unipolar e o Bipolar, o mesmo será Unipolar quando este possuir dois enrolamentos por fase, sendo um para cada sentido, já o do tipo Bipolar sera quando ele tiver apenas um enrolamento por fase.

O servo motor de Passo tem como vantagens o fato de ser compacto, precisão no posicionamento e o controle de aceleração e desaceleração podendo assim ser uma alternativa viável em projetos quando algo tem que ser posicionado muito precisamente ou rodado de um ângulo exato.

![Servo Motor De passo](/42/images/post/Servo Motor de passo.jpg)

Um servo motor cc é basicamente um conjunto de um pequeno motor de corrente contínua,uma caixa de engrenagem,um potenciômetro de realimentação e pelo circuito eletrônico do acionamento e loop de controle.

O servo motor CC tem como vantagem a operação em 4 quadrantes com custos relativamente mais baixos, ciclo contínuo mesmo em baixas rotações, Ampla variação de velocidade e o Alto torque na partida e em baixas rotações. As desvantagens seriam a Maior necessidade de manutenção (devido aos comutadores), também tendo o problema dos arcos e faíscas devido à comutação de corrente por elemento mecânico (não podendo ser utilizado em ambientes perigosos). O servo motor CC pode ser utilizado em projetos como monitoramento do fluxo de ar de refrigeração e também Pintura em cor espacial.

![Servo Motor CC](/42/images/post/Servo Motor CC.jpg)

### Servo Motor CA

Existem dois tipos distintos de Servo Motor CA: síncrono e de indução.

O motor de indução possui tem seu motor construído de alças de fio encurtadas em uma armadura giratória. Eles são robustos, versáteis e podem fornecer potência considerável, sendo mais encontrados em aplicações maiores pois não possuem bom rendimento a baixas potências. Tem como vantagem o alto torque, boa eficiência operacionale e baixa manutenção. Um dos maiores impecilhos seria seu custo elevado, fazendo com que o mesmo não seja tão acessivel.

O servo motor síncrono é o mais encontrado na indústria e é composto de estator e rotor.  Seu gerador eletrico consiste basicamente em uma estrutura cilíndrica e núcleo, sendo que a bobina de indução é enrolada em volta do núcleo do estator e a extremidade da bobina é ligada a um fio condutor através do qual é fornecida corrente ao motor. Suas vantagens seriam os altos picos de torque, a boa eficiência oprecional, baixa manutenção e durabilidade alta. Suas desvantagens seriam seu controle complexo e o custo elevado, mostrando assim que o servo motor CA de Indução e sincrono apresentam os dois um custo elevado.

![Servo Motor CA](/42/images/post/Servo Motor CA.jpg)

#### Referências

SILVEIRA, Cristiano Bertulucci. Servo Motor: Veja como Funciona e Quais os Tipos. In: Servo Motor: Veja como Funciona e Quais os Tipos. [S. l.], 20--. Disponível em: https://www.citisystems.com.br/servo-motor/. Acesso em: 18 nov. 2019.

ARAÚJO, Thayron. Série Motores: Introdução ao Motor de Passo. In: Série Motores: Introdução ao Motor de Passo. [S. l.], 19 nov. 2019. Disponível em: https://blog.fazedores.com/serie-motores-introducao-ao-motor-de-passo/. Acesso em: 18 nov. 2019.

MOTA, Allan. O que é Servomotor? Controlando um Servo com Arduino. In: O que é Servomotor? Controlando um Servo com Arduino. [S. l.], 20--. Disponível em: https://portal.vidadesilicio.com.br/o-que-e-servomotor/. Acesso em: 18 nov. 2019.
