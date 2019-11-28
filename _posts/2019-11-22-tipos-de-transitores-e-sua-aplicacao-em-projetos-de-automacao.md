---
layout: post
title: "Tipos de transitores e sua aplicação em projetos de automação"
categories: ['Automação']
authors: ['Camila Coelho Lopes'] 
tags: []
description: ''
image: trans.jpg
---

### SURGIMENTO DOS TRANSISTORES

Em 16 de dezembro de 1947 foi desenvolvido primeiro transistor. Nessa época os transistores substituíram, por serem mais compactos, robustos e eficientes as válvulas nas aplicações eletrônicas. Os transistores são tão importantes que (BRAGA, 2016) diz que se hoje temos computadores pessoais, telefones celulares, e muitos outros equipamentos eletrônicos compactos e baratos foi justamente graças a invenção do transistor. 

Os diodos semicondutores, de estado sólido, já eram conhecidos antes 1920, como por exemplo, os retificadores de óxido de cobre. Muitos pesquisadores começaram a questionar sobre controlar uma corrente num retificador, a partir de algum eletrodo colocado em sua estrutura, depois da invenção da válvula tríodo, pois isso permitiria elaborar um dispositivo de estado sólido capaz de amplificar correntes assim como faria a válvula tríodo. A ideia não era descartável, porém os pesquisadores não descobriram muita coisa, já que os materiais usados na produção dos diodos eram inapropriados para isso. Hoje em dia os transistores são produzidos normalmente em germânio e em silício através da adição de impurezas.

### TRANSISTORES

Os transistores são, segundo (PIROBO, 2017) o substituto da válvula eletrônica, dispositivos semicondutores de três camadas. Os transistores são muito utilizados na construção de chips eletrônicos. Eles substituíram as válvulas, pois além de amplificar uma corrente elétrica eles podem ser usados em circuitos onde assumem apenas os dois extremos, sendo totalmente “fechados” ou totalmente “abertos”. Exemplificando, em uma função idêntica à dos interruptores comuns, destes usados para acender lâmpadas, podem ser ajustados apenas para interromper inteiramente uma corrente elétrica (se “fechado”) ou para deixá-la passar integralmente (quando “aberto”).
	
Na pratica os transistores funcionam da seguinte forma: A um transistor são ligados três terminais que recebem o nome de “emissor”, “coletor” e “base”. Um emissor e um coletor que estão conectados a um circuito elétrico em série que pode ou não ser alimentado por uma corrente. Uma base é ligada a outro ponto do circuito cuja finalidade é controlar o estado do transistor. Quando uma tensão elétrica é aplicada à base, o transistor “abre”, ou seja, funciona como condutor, permitindo que uma corrente elétrica flua entre emissor e coletor e alimente o circuito ao qual está ligado. Quando a tensão aplicada à base é nula, o transistor “fecha” e se comporta como um isolante, impedindo o fluxo da corrente e cortando a alimentação do circuito.

Segundo (MATIAS, 2013), o funcionamento do transístor pode ser comparado a uma torneira de água que, quando a sua válvula está mais ou menos aberta, ela deixa passar, respectivamente, mais ou menos quantidade de água – no caso do transístor, será mais ou menos corrente elétrica.
Tipos De Transistores

Ha dois tipos de transistores atualmente, os transistores bipolares e os unipolares. O BJT (Bipolar Junction Transístor) transístor bipolar é o mais utilizado atualmente, sendo o que foi fabricado primeiro. Os unipolares ou, como também são conhecidos, os FET (Field Effect Transístor). Os FET por sua vez são subdivididos em algumas variantes, sendo estas: o JFET (Junction Field Effect Transístor), o mosfet (Metal Oxid Semiconductor Function Effect Transistor ), o Nmosfet (tipo n), o Pmosfet (tipo p).

### TRANSISTORES BIPOLARES

Ele é constituído por duas junções PN ligadas entre si, assim pode-se obter configurações diferentes: o transístor NPN é uma junção de NP e PN e o transístor PNP é uma junção de PN + NP. Destas junções resultam três zonas de condução, às quais foram dados os nomes de Coletor (C), Base (B) e emissor (E), que haviam sido vistos a cima. A Base se dá como a região intermédia entre o Coletor e o Emissor, que por sua vez ficam nos extremos; o Emissor difere do Coletor por ter mais impurezas do que este. O transístor, então, fica por possuir duas junções, sendo designadas por Coletor-Base e Base-Emissor.

As duas configurações de transistores bipolares (NPN e PNP) possuem alguns princípios de funcionamento semelhantes, porém com suas tensões aplicadas simétricas entre si, ou seja, cada transístor NPN pode ter um transístor PNP equivalente ou complementar. São os casos, por exemplo, dos seguintes pares de transístores: 2N3904 (NPN) e 2N3906 (PNP) ou BC548 (NPN) e BC558 (PNP), entre muitos outros.

O transístor (NPN ou PNP) apresenta exteriormente três terminais (três patas) que estão ligadas internamente a cada uma das três zonas de condução do transístor. O datasheet ou folha de dados de cada transístor indica quais são os terminais de cada transístor, pelo que é sempre necessário consultá-lo em manual técnico ou no site do fabricante, na Internet.

### TRANSISTOR UNIPOLAR 

O transistor unipolar ou de efeito de campo (FET) é o nome dado aos transistores, que funcionam por tensão e não por corrente como normalmente os transistores bipolares são! Esses transistores possuem 3 regiões: UMA PORTA, UMA FONTE E UM DRENO, também possuem uma alta taxa de resistência e impedância de entrada, essa última faz com que os FET 's tenha uma quantidade muito pequena de corrente passando através dele, por esse motivo tiram níveis mínimos de corrente da fonte de alimentação de um circuito, o que impede que haja uma sobrecarga.

O FET consiste num canal formado por semicondutores que transportam a corrente elétrica, onde sua condutividade é controlada pela tensão que é aplicada no seu exterior, devido a esse fato, esses transistores podem amplificar ou anular a tensão de um circuito.
Atualmente encontramos variantes desses transistores sendo o JFET (Transistor de Junção por Efeito de Campo) e MOSFET (Transistor de Efeito de Campo de Óxido de Metal Semicondutor) os 2 principais encontrados no mercado. O JFET têm uma impedância elevada, e por isso são utilizados em equipamentos de alta impedância de entrada, possui os canais básicos N e P, trabalha com a PORTA inversamente  polarizada e possuem uma tensão de saturação bem próxima de zero para  correntes Drain – Source pequenas, já os MOSFET são transistores de porta isolada, ou seja, o MOSFET possui uma película de óxido que isola a região do canal que liga a região do dreno com a região da fonte, e dependendo de sua polaridade de seus semicondutores teremos o canal N ou P.

### ALGUMAS UTILIZAÇÕES PRÁTICAS DO FET

Acionador de relé com o MOSFET: Quando há luz sobre a célula, sua resistência é baixa, desligando. Quando a luz se apaga, a resistência é alta, acionando.
Circuito temporizador com JFET: Quando a chave está fechada a tensão da porta torna-se 0V e a corrente da região do dreno resultante é IDSS e a lâmpada acende por completo. Quando solta o capacitor carrega-se até -9V, e quando atingido a Vp, o Transistor JFET desliga, juntamente com a lâmpada o tempo em que a lâmpada está liga e determinada por 

τ = (R1 + R2) C e Vp.

### ZONAS DE OPERAÇÃO DE TRANSISTORES

Existem 4 zonas de operação de um transistor, sendo elas:
1. Zona ativa: Utilizado como amplificador
2. Zona de Corte: Utilizado como chave, ou seja, funciona como um interruptor! A zona de corte funciona como um interruptor aberto, isso ocorrerá quando o coletor for igual a nulo. Nesse caso IB ≅ 0.
3. Zona de Saturação: Também é utilizado como chave! A zona de corte funciona como um interruptor fechado, isso ocorre quando a corrente entre o emissor e o coletor são nulas e a corrente do coletor atinge seu nível máximo. IC = VCC / RC
4. Zona de Ruptura: Região proibida, onde o transistor não pode operar caso o contrário será danificado, isto é, seu valor máximo de tensão ultrapassado quando da operação dessa zona.

---

### Referências

SANTOS. Antonio. Elementos de Eletrônica Analógica. 2019. Disponível em: [https://www.if.ufrj.br/~toni/analogica8.pdf](https://www.if.ufrj.br/~toni/analogica8.pdf) Acessado em 19 de nov. de 2019.

Transistor: Princípios de Funcionamento e Aplicações. Portal Eletricista. 2014.  Disponível em: [https://www.portaleletricista.com.br/transistor-funcionamento-e-aplicacoes/](https://www.portaleletricista.com.br/transistor-funcionamento-e-aplicacoes/) Acessado em: 19 de nov. de 2019.

NICOLLET. Aparecido. Aula 15 Aplicações Práticas dos FETs. 2017. Disponível em: [https://www.pucsp.br/~elo2eng/Aula_15_2017.pdf](https://www.pucsp.br/~elo2eng/Aula_15_2017.pdf) Acessado em: 19 de nov. de 2019.

M042 - O Transistor Jfet Como funciona o transistor Jfet?. EletronPi. 2019. Disponível em: [http://www.eletronpi.com.br/ce-042-transistor-jfet.aspx](http://www.eletronpi.com.br/ce-042-transistor-jfet.aspx) Acessado em: 19 de nov. de 

BRAGA. Newton. Como funciona o MOSFET (ART977). 2019. Disponível em: [https://www.newtoncbraga.com.br/index.php/como-funciona/6417-art977](https://www.newtoncbraga.com.br/index.php/como-funciona/6417-art977) Acessado em 19 de nov. 2019.

O transistor uniporlar. ybites.Disponível em: [https://www.ibytes.com.br/o-transistor-de-efeito-de-campo-as-vezes-e-chamado-transistor-unipolar/](https://www.ibytes.com.br/o-transistor-de-efeito-de-campo-as-vezes-e-chamado-transistor-unipolar/). Acesso em: 19 de novembro de 

Transistor, o que é? Tipos e como funciona!. Papel Digital. Disponível em: [https://www.palpitedigital.com/transistor-tipos-como-funciona/](https://www.palpitedigital.com/transistor-tipos-como-funciona/). Acesso em: 19 de novembro de 2019
 
MATIAS. José. Oque é um transistor?. Disponível em: [http://www.josematias.pt/eletr/o-que-sao-transistores/](http://www.josematias.pt/eletr/o-que-sao-transistores/). Acesso em: 19 de novembro de 2019
 
PIROPO. B. Transistor para principiantes. Disponível em: [https://www.techtudo.com.br/artigos/noticia/2012/07/transistores-para-principiantes.html](https://www.techtudo.com.br/artigos/noticia/2012/07/transistores-para-principiantes.html). Acesso em: 19 de novembro de 2019

O que é e para que serve um transistor?. Mundo da elétrica. Disponível em: [https://www.mundodaeletrica.com.br/o-que-e-e-para-que-serve-um-transistor/](https://www.mundodaeletrica.com.br/o-que-e-e-para-que-serve-um-transistor/). Acesso em: 19 de novembro de 2019

Transistor. Brasil Escola. Disponível em: [https://brasilescola.uol.com.br/fisica/transistor.htm](https://brasilescola.uol.com.br/fisica/transistor.htm). Acesso em: 19 de novembro de 2019

