# 42
Site com todas as respostas do universo

## Como contribuir

Se você faz parte do time, siga as instruções abaixo normalmente. Se você não faz parte, faça um _fork_ do projeto e trabalhe a partir do seu próprio repositório, depois solicite um Pull Request para este aqui.

0. Instale o Node.JS
1. Instale o [Docker](https://docker.com)
2. Clone este repositório
3. Crie sua branch
3. Inicie o servidor
4. Utilize um editor de texto
5. Envie suas modificações
5. Faça um Pull Request

### Instale o Node.JS

Baixe o [Node.JS](https://nodejs.org) a partir do site oficial e siga as instruções do site.

### Instale o Docker

Se você utiliza distribuições **Linux**, utilize seu gerenciador de pacotes para baixar e instalar o Docker. Em versões baseadas em Debian (como Ubuntu) execute:

```bash
$ sudo apt install docker
```

Se você utiliza **Windows**, então instale o [VirtualBox](https://www.virtualbox.org), baixe o [Boot2Docker](https://github.com/boot2docker/boot2docker) e siga as [instruções de instalação](https://github.com/boot2docker/boot2docker#installation).

Se você utiliza **Mac OS**, baixe e instale o [Docker Desktop for Mac](https://hub.docker.com/?overlay=onboarding).

> No Windows só compensa utilizar o Docker Desktop apenas se você for capaz de gerenciar máquinas Hyper-V, pois é necessário criar Contâiners Linux.

### Clone este repositório

```bash
$ git clone https://github.com/ifroariquemes/42.git
```

### Crie sua branch

**Entre na pasta do projeto** e execute:

```bash
$ git branch um-nome-qualquer
$ git checkout um-nome-qualquer
```

### Inicie o servidor

```bash
$ npm run start
```

### Utilize um editor de texto

Use qualquer editor de texto de sua preferência para criar postagens. Utilize qualquer arquivo da pasta `_posts` como base para escrever seu próprio post. 

Esta é a estrutura mínima de um post:

```Markdown
---
layout: post
title: 'Titulo do Post'
categories: ['Cat1', 'Cat2']
authors: ['Seu Nome']
tags: ['Palavras', 'Chave']
description: 'Pequeno resumo sobre a postagem'
image: 'image_de_destaque.jpg'
---
Texto da postagem
```

Todos os post devem ser escritos em Markdown, com a estrutura acima que faz parte do front-matter do Jekyll. Veja o guia a seguir para aprender a escrever para o site:
[Markdown Cheatsheet by Adam](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

### Envie suas modificações

**Dentro da pasta raiz do projeto**, execute:

```bash
$ git add _posts
$ git add images
$ git commit -m "conte o que voce fez"
$ git push -u origin um-nome-qualquer
```

### Faça um Pull Request

Solicite a um administrador que avalie suas modificações e considere incluir seu post no site oficial. Para isto, no Repositório do GitHub, altere a branch para aquela criada anteriormente e selecione o botão ao lado `New Pull Request`.

Preencha o formulário e aguarde a avaliação do revisor. Obrigado por contribuir!