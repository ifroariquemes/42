---
layout: post
title: "Uso do Gerenciador de Tarefas"
categories: ['Manutenção']
authors: ['Renato Lopes'] 
tags: ['Gerenciador de Tarefas', 'Windows tarefas', 'task maneger']
description: 'Aprenda a utilizar os recursos deste programa poderoso do Windows'
image: logo.png
---
# Abrir o gerenciador de tarefas
O gerenciador de Tarefas foi criado em 1993 no Windows NT, para  a facilitação de administração de tarefas, a ferramenta sofreu processos de modificação até o atual Windows 10.

Para acessar a opção do gerenciador de tarefa, basta utiliazar o atalho ctrl + shift + esc,

Outras formas de acessar o Gerenciador de Tarefas:
* R + Windows e digitar "taskmgr"
* Ctrl + Alt + Del 
* Botão direito na barra de tarefas, clique em gerenciador de tarefas.

---

# Panorama Comum do gerenciador de tarefas
Após a abertura do gerenciador de tarefas é comum que se encontre apenas uma lista de tarefas, sem mais detalhes, tendo apenas as opções **"Finalizar"** e **"Mais detalhes"**.
clique em "Mais detalhes" para ter um panorama geral, lógo em seguida deve ser mostrado as abas **Processos**, **Desempenho**, **Histórico de aplicativo**, **Inicializar**, **Usuários**, **Detalhes** e **Serviços**

---

# Processos, detalhes e serviços.
A lista de processos tem habitualmente três listas de categorias principais: **Aplicativos**, **Processos em segundo plano** e **Processo do Windows**.

* Aplicativos: são os aplicativos rodando  que estão abertos, eles costumam a aparecer na barra de tarefas.

* Processos em segundo plano: São os aplicativos da Windows Store, ou softwares sendo rodados em subplanos, ou quando uma tarefa é agendada.

* Processos do Windows: Como já dito no próprio nome são os processos principais e fundamentais no funcionamento do Windows que estão sendo rodados no Windows "debaixo dos panos".
![](/42/images/post/ProcessosNormal.jpeg)

Ao clicar com o botão direito do mouse em qualquer processo, você tera as opções: **expandir**, **finalizar tarefa**, **enviar comentários**, **valores de recurso**, **Criar arquivo de despejo**, **Ir para detalhes**, **Abrir local do arquivo**, **Pesquisar online**, **Propriedades**.
![](/42/images/post/InfoProcessos.jpeg)

* Expandir: Mostra todos os sub-processo que estão rodando no aplicativo.
* Finalizar Tarefa: finaliza e fecha o processo em execução (Não recomendado caso seja um processo importante).
* Enviar Comentários: Serve para enviar comentários a respeito do software, relatando erros, ou problemas.
* Valores de recursos: onde mostrara **Memória**, **Disco** ou **Rede**, e lá podera escolhar se os dados citados acima poderão ser modificados para serem apresentados ou em **Valores** ou em **Porcentagens**.
![](/42/images/post/ValoresDeR.jpeg)
* Criar arquivo de despejo: é uma ferramenta preferencial para programadores, ele irá pegar todas as coisas usadas na memória RAM, e gravar em um local no disco.
![](/42/images/post/ArquivoDeDespejo.jpeg)
* Ir para detalhes: Será redirecionado para detalhes e mostrara onde o serviço selecionado está.
* Abrir local do arquivo: Levará até onde o aplicativo está salvo no dísco.
* Pesquisar online: Faz uma pesquisar com o nome do executavel(.exe), sendo aberto no Bing.
* Propriedades: É onde mostrara as informações gerais do aplicativo, como tamanho ou local onde está armazenado no dísco.
![](/42/images/post/Propriedades.jpeg)

---

# Desempenho
No Windows 10, desempenho é mostrado em tempo real, com um gráfico. São mostradas as informações **CPU**, **Memória**, **Dísco**,**Wifi** ou **Ethernet**, e caso você tenha uma GPU que não seja integrada, ela também aparecera na gráfico com **GPU**.
![](/42/images/post/Desempenho.jpeg)

* CPU: Na parte superior direita será mostrado o nome da sua CPU e a sua velocidade. Em baixo mostra o quanto está sendo usado da sua CPU, e a velocidade em que ela se encontra. É mostrado também as informações do processador assim como também é mostrado as informações de trabalho.
* Memória: No painel superio é mostrado o quanto de RAM você tem e o quanto está sendo usado.
* Dísco: Assim como os outros,é mostrado um gráfico de atividades, que mostra a taxa de transaferencia do dísco, e a atividade dele, atualizada a cada 60 segundos. tambem é mostrado informações como tempo de atividade e tempo médio de respostas.
* Wi-Fi/Ethernet: Mostra a vélocidade de download e upload qe está na sua rede, assim como também mostra as informações de sua conexão.
* GPU: Há vários gráficos de informações para váriadas coisas, como 3D, Uso de memória dedica e de memória compartilhadas.Você também pode ver Qual o modelo de sua GPU e sua versão de dríver.

![](/42/images/post/InfoDesempenho.jpeg)

Também há **Exibição resumida**, **Ocultar gráfico** e **Copiar** 

* Exibição resumida:Só mostrará O gráfico principal sem os dados no lado direito da tela.
* Ocultar gráfico: Ira remover os gráficos principais e deixar em seu lugar um ícone redondo.
* Copiar: Copiara as informações a qual foi escolhido e os dadosestarão salvos no exato momentoem que foi copiado.

---
# Histórico de aplicativos.

Onde é mostrado os últimos aplicativos usados no seu PC, porém, aparecera apenas os reconhecidos da Microsoft.

![](/42/images/post/HIstoricoAplicativos.jpeg)

---

# Inicializar
É por onde você pode escolher os aplicativos que se iniciam após o Windows ligar, e também pode fazer o processo reverso e desabilitar.

![](/42/images/post/Inicializar.jpeg)

Em **status** é mostrado quais estão habilitados e desabilitados.

---

# Usuários  
É uma lista com usuários que estão conectados em seu pc, mostrando os mesmos dados que continha em processos.

![](/42/images/post/Usuarios.jpeg)

É possivel gerenciar as contas que lá se encontram, apenas apertando o botão direito do mouse e clicando em gerenciar contas de usúarios. Assim como também pode ser expandido e desconectado

![](/42/images/post/InfoUsers.jpg)

---

# Detahes
É o paínel que contém mais detalhes, aqui haverá mais funções e informações que na aba **Processos**

![](/42/images/post/Detalhes.jpeg)

As operações que nele podem ser realizadas são: **Finalizar tarefa**, **Finalizar Árvore de processoss**, **Definir prioridade**, **Definir afinidade**, **Analisar cadeia de espera**, **Virtualização do UAC**, **Criar arquivo de despejo**, **Abrir local do arquivo**, **Pesquisar online**, **Propriedades** e **Ir para serviço(s)**.

![](/42/images/post/infoDetalhes.jpeg)

* Finalizar tarefa: Finalizara o processo.
* Finalizar Árvore de processos: Finalizara toda a cadeia dentro daquelo serviço.
* Definir prioridade: Definira a prioridade do processo como: Baixa, Abaixo do normal, Normal, Acima do Normal, Alta e Tempo real. os processos normalmentese encontram na prioridade normal, no entanto, os processos de prioridades altas devem ser os necessários para o funcionamento do desktop, já os opostos para aplicativos de segundo plano.
* Definir afinidade: deixara aquele processo para um processador fazer apena um thread nele.
* Analisar cadeia de espera: Mostra quais threads estão em espera, ou seja, quais threads estão aguardando para usar um recurso ou ferramenta.
* Virtualização do UAC: Função para ativar ou desativar a virtualização do controle de contas, pode ser usado para correção de acesso a arquivos de sistema, que muda o acesso ao arquivo eregistro para outra pasta.
* Criar arquivo de despejo: Captura a memória daquele arquivo(.exe) e salva em uma pasta do sistema.
* Abrir local do arquivo: Levara até onde o arquivo está salvo no dísco.
* Pesquisar online: Fara uma pesquisa desta aplicação (.exe) no bing.
* Propriedades: Mostra as informações do arquivo (.exe).
* Ir para serviço(s): Levara até os registros que estão associados ao processo na guia de serviços.

---

# Serviços
A aba de serviços é onde será mostrado os serviço do sistema operacional Windows. Evite mexer nesta aba a não ser que saiba o que está fazendo, e nem é uma aba para usúarios comuns.

![](/42/images/post/servicos.jpeg)