---
layout: post
title: "A automação ajudando os deficientes visuais"
categories: ['Automação']
authors: ['Jocássia Dolci'] 
tags: ['Automação','Acessibilidade','Cinto'.]
description: 'O presente post apresentará dispostivos desenvolvidos para auxíliar deficientes visuais'
image: aut.jpg
---

A tecnologia também abre portas para o aumento e desenvolvimento da acessibilidade, possibilitando a criação de dispositivos e sistemas. Existem vários projetos com esse intuito, dos quais alguns serão citados no presente post.

### Cinto: Dispositivo de auxílio a deficientes visuais

Neste projeto, estudantes do Colégio Nossa Senhora da Aparecida se propuseram a desenvolver um dispositivo de baixo custo, que seja simples e adaptável. Escolheram então desenvolver um cinto que se ajusta ao corpo do usuário. Para desenvolve-lo, eles utilizaram:

* Microcontrolador: O microcontrolador escolhido foi o Arduino, por ser uma
plataforma open-source com hardware e software acessíveis. 

* Sensores Ultrassônicos: Os sensores ultrassônicos utilizados (Modelo HC-SR04)
apresentam peculiaridades decorrentes de sua escolha. Estes apresentam uma boa precisão, um maior alcance, conseguindo aferir leituras entre 0.3 e 4 metros, poucas interferências externas e apresentam fácil comunicação com o microcontrolador.

* Motores de Vibração: Os motores de vibração produzem um retorno tátil e são de
fácil acesso.

* Bateria: A bateria escolhida para alimentar todo o projeto foi do tipo
Lítio-Polímero (7.4V – 730mAh) por ser leve, pequena e com
ótima autonomia, aproximadamente 6 horas de uso

* Placa de Circuitos: Para a conexão dos sensores e do microcontrolador, foi
produzida, com a ajuda do software Eagle, uma placa de
circuitos.

#### Funcionamento 

Foi elaborado um algoritmo que analisa a distância encontrada pelos sensores ultrassônicos para checar a relação entre o espaço disponível para locomoção. Caso perceba-se que esse espaço está diminuindo, significando que existe algum obstáculo à frente, os motores de vibração começarão a funcionar, fornecendo um retorno tátil para o deficiente.

Legal, né!!


### A grande MIT também participa!

Uma equipe de engenheiros do Laboratório de Ciência da Computação e Inteligência Artificial (CSAIL) do MIT desenvolveu um aparelho vestível para ajudar deficientes visuais em sua vida cotidiana. O aparelho consegue reconhecer obstáculos e transmite essa informação aos usuários por meio de uma série de motores vibratórios que ficam localizados na região da sua cintura.

Ele é composto por uma câmera de profundidade, uma interface reprogramável em Braille e o cinto com motores vibratórios. A câmera consegue identificar superfícies e outros obstáculos, e avisa o usuário quando ele está próximo deles por meio de vibrações localizadas. A intensidade e a localização das vibrações ajudam a pessoa a saber com precisão onde estão os obstáculos.

Os primeiros testes realizados com deficientes visuais deram resultados bastante positivos: as pessoas que usaram o aparelho para caminhar pelos corredores do MIT reduziram em 86% o número de contatos acidentais, na comparação com quem estava usando apenas uma bengala dobrável. 

Por outro lado, o aparelho ainda está em fase inicial de testes, como ressalta o TechCrunch. Os pesquisadores ainda não têm um cronograma de desenvolvimento até um produto final, mas esperam que o dispositivo possa um dia ser usado como substituto para as bengalas tradicionalmente usadas por deficientes visuais.

Existe uma gama de dispositivos no mercado, até mesmo casas adaptadas para deficientes visuais. A automação nos permite ajudar a todos, basta investimento e criatividade!!

----------------------------------------------
REFERÊNCIAS

CARVALHO, Ítalo Lélis de et al. **CINTO: DISPOSITIVO DE AUXÍLIO A DEFICIENTES VISUAIS**. 2013. Disponível em: <http://sistemaolimpo.org/midias/uploads/12a54f961eb531d15e915497a262ae28.pdf>. Acesso em: 22 nov. 2019.

SUMARES, Gustavo. **MIT cria aparelho vestível para auxiliar deficientes visuais**. 2017. Disponível em: <https://olhardigital.com.br/noticia/mit-cria-aparelho-vestivel-para-auxiliar-deficientes-visuais/68770>. Acesso em: 22 nov. 2019.
