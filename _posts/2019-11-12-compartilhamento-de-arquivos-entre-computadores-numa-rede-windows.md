---
layout: post
title: "Compartilhamento de arquivos entre computadores numa rede Windows"
date: 2019-11-12 09:20
categories: ['Manutenção']
authors: ['Gabriel Bitencourt Marin'] 
tags: ['Rede', 'Windows', 'Compartilhar', 'Arquivos', 'Computador']
description: 'Tutorial de como compartilhar seus arquivos em uma rede utilizando windows 10'
image: using-computer.jpg
---

As vezes é necessário compartilhar algum arquivo importante entre dois ou mais computadores. Pode acontecer dos computadores não estarem conectados à intenet ou não terem alguma conexão além da rede local. Felizmente o Windows tem uma funcionalidade que possibilita o compartilhamento de arquivos em uma rede local.

## Ative o compartilhamento

É preciso primeiro verificar se compartilhamento de arquivos está ativado.

1. Clique com o botão direito no ícone de conexão e clique em "Abrir configurações de rede e internet".
![Imagem1](/42/images/post/compartilhar-arquivos-windows(1).png)

2. Se você estiver em uma rede doméstica ou do trabalho, verifique se ela está marcada como privada, se não estiver vá em "Alterar as propriedades de conexão" e marque "Particular", depois volte até a aba "Status" em "Rede e Internet".
![Imagem2](/42/images/post/compartilhar-arquivos-windows(2).png)

3. Clique em "Opções de compartilhamento".

4. Se estiver em uma rede privada selecione "Particular" senão selecione "Convidado ou Público".
5. Em "Descoberta de rede" clique em "Ativar descoberta de rede" e em "Compartilhamento de arquivos e impressora" clique em "Ativar compartilhamento de arquivo e impressora".
![Imagem3](/42/images/post/compartilhar-arquivos-windows(3).png)

6. Por padrão o Windows pede uma senha quando alguém tenta entrar em um pasta compartilhada. A senha pode ser desativada indo em "Todas as Redes" e selecionando "Desativar compartilhamento protegido por senha".
![Imagem4](/42/images/post/compartilhar-arquivos-windows(4).png)

7. Clique em "Salvar alterações".

## Compartilhe uma pasta

Agora que o compartilhamento de arquivos está ativado você poderá compartilhar suas pastas na rede.

1. Localize a pasta que você queira compartilhar, clique com o botão direito sobre ela, em "Conceder acesso a", clique em "Pessoas específicas".
![Imagem5](/42/images/post/compartilhar-arquivos-windows(5).png)

2. Em "Escolha as pessoas com as quais irá compartilhar" selecione "Todos" e clique em "Adicionar".
![Imagem6](/42/images/post/compartilhar-arquivos-windows(6).png)

3. Em nível de permissão você pode alterar as permissões dos outros usuários quanto a pasta que você compartilhou. "Leitura" para dar permissão para poder apenas ver a pasta ou "Leitura/Gravação" para permitir que as outras pessoas modifiquem o conteúdo da sua pasta.
![Imagem7](/42/images/post/compartilhar-arquivos-windows(7).png)

4. Clique em "Compartilhar".

5. Você pode copiar o link da sua pasta compartilhada para que as outras pessoas possam alterar ou adicionar arquivos em sua pasta.
![Imagem8](/42/images/post/compartilhar-arquivos-windows(8).png)

Pronto! Para acessar a pasta compartilhada abra o Windows Explorer e cole o link na barra de endereço ou vá até "Rede" no Windows Explorer e procure pela pasta compartilhada.
