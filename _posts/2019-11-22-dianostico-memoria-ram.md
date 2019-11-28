---
layout: post
title: "Diagnóstico de Memória RAM"
categories: ['Manutenção']
authors: ['Nalbert Mancini de Andrade'] 
tags: []
description: 'Descubra se sua memória está com defeito com o MemTest86'
image: board-22098_1280(1).jpg
---
### Apresentação
___

O diagnóstico de memória é uma ação fundamental para o bem estar de seu computador, ele pode te apontar erros atuais, possíveis erros, problemas, soluções  e entre outros.

Para esse processo usaremos um programa chamado **MemTest86**, pode ser obtido de forma gratuita no site oficial <https://www.memtest86.com/download.htm>,  nesse site você terá a opção de escolher duas versões de forma gratuita, V4 e V8. Para a escolha da versão deve se saber que V8 funcionará apenas se tiver inicialização com UEFI, para isso deve verificar o site oficial de do fabricante de sua placa mãe e verificar se há ou não esse recurso, caso o seu computador não tenha esse recurso baixe a versão antiga, a V4. Na iso haverá um manual sobre o MemTest86.

### MemTest86

___

O MemTest86 é um programa independente, não requer um sistema operacional para seu funcionamento, porém para seu funcionamento deve-se utilizar um hardware que possa ser usado como meio de boot, um disco ou pendrive, para isso você deve utilizar um sistema operacional, Windows, Linux ou Mac, para que você possa instalar o programa. Você deve inicializar o seu computador com o hardware que está sendo utilizado como meio de boot, para isso você deve trocar a ordem de boot de seu computador.

* As versões têm métodos de interação diferentes, o V8 tem a interface  melhor e mais fácil para o trabalho em relação ao V4, porém ambos têm como padrão  inicializar com o teste de memória. O V8 mostra informações do seu computador, assim como o V4 porém em 
repartições, o V8 não inicia já fazendo o teste, há opções relacionados ao teste, como escolher qual pente de memória fazer o teste, porém, ainda sim todas as informações contidas neste site, exceto questão de localização da tela, são referentes ao MemTest86 V8.
 

### Como Usar e Informações

___

Na interface do MemTest86 V4 há vários componentes relacionado ao seu computador e, principalmente, a sua memória RAM. Entre eles há informações sobre cada memória em cada slot no computador, como modelo e tipo, no campo “Memory SPD informations “. No primeiro campo superior direito há informações de sua memória, como tamanho e velocidade da memória cache e da memória como um todo. Ao lado Direito há informações do processo da atividade e informações de seu computador, como o tipo de seu processador e velocidade, há informações de porcentagem da atividade, qual teste está sendo executado, eles são numerados a partir de 1, a parte da memória que está sendo testada e o tempo de execução. Abaixo há uma carreira de campos, do lado esquerdo para o lado direito, no primeiro mostra informações de seu processador, como a numeração de cada um, a partir do 0, os estaus, quantos cores está sendo utilizado do total, e temperatura. No segundo há informações de sua memória, como tamanho, velocidade, tipo, modelo, a quantidade de erros e a quantidade de testes completos.

![memtest](/42/images/post/memtest.png)

Para o entendimento do programa é necessário da leitura do manual que vem incluso na iso baixada. Sobre o relatório de erros, ao final de cada teste finalizado é criado um código em HTML no disco, que, posteriormente, é possível abri-lo e visualizar o relatório de erro. Entre os erros há:

###### Menor erro de endereço:

Tecnicamente é o menor endereço que foi encontrado um erro.
###### Maior erro de endereço:

Tecnicamente é o maior endereço que foi encontrado um erro.
###### Bits com erro Mask:

Uma máscara de todos os bits com erro em hexadecimal.
###### Bits com erro:

Bit total com erro para todas as instâncias de erro e os minutos. Bit máximo e médio com erro de cada ocorrência individual.
###### Máximo de erros contínuos:

O máximo de endereços contínuos com erros.
###### Erros de teste:

O número de erros para cada teste é exibido.

___

Bem abaixo na interface há uma lista de comandos, como “esc” que sai do programa, “(C)” que abre as configurações, “(SP)” que trava a tela,”(CR)” que  destrava a tela. Há também comandos como “F2” que ativa todos os cores do processadores (pois que inicialmente é usado apenas 1). Em configurações há as seguintes opções:

###### Configurações:

|(1)|Seleção de Teste|
|(2)|Intervalo de Endereços|
|(3)|Modo de Relatório de Erros|
|(4)|Seleção do Núcleo|
|(5)|Atualizar Tela|
|(6)|Exibir dados DMI|
|(7)|Exibir dados SPD|
|(0)|Continuar|



Os mais interessantes são o 3 que pode te avisar quando aparecer um erro e o 6 que mostra os canais que a placa-mãe possui.


