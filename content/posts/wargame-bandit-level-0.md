---
title: "WarGame Bandit Level 0"
date: 2021-09-27T20:54:15-03:00
draft: false
# weight: 1
# aliases: ["/first"]
tags: ["WarGames", "Bandit", "Linux"]
categories: ["Over the wire"]
author: "Angelo Morette"
# author: ["Me", "You"] # multiple authors
showToc: true
TocOpen: false
hidemeta: false
comments: false
description: "Primeiro nível do desafio, conseguir conectar via ssh ao bandit.labs.overthewire.org"
canonicalURL: "https://canonical.url/to/page"
disableHLJS: true # to disable highlightjs
disableShare: false
disableHLJS: false
hideSummary: false
searchHidden: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
cover:
    image: "<image path/url>" # image path/url
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
---

https://overthewire.org/wargames/bandit/bandit0.html

## Meta

> The goal of this level is for you to log into the game using SSH. The host to which you need to connect is bandit.labs.overthewire.org, on port 2220. The username is bandit0 and the password is bandit0. Once logged in, go to the Level 1 page to find out how to beat Level 1.

## Comando para resolver o problema

> ssh

### O que é ssh?

ssh (Secure Socket Shell) é um protocolo que permite ao usuário acessar uma máquina de forma remota.

## Write up

* Nome do host: `bandit.labs.overthewire.org`
* Nome do usuario: `bandit0`
* Senha: `bandit0`
* Porta: `2220`

### Para Usuários Linux

**Passo 1:** Abra o terminal.

**Passo 2:** Digite o comando nessa estrutura para conectar.

> ssh [usuário]@[nomeHost] -p [porta]

**Passo 3:** Digite a senha e precione `enter`.

**Passo 4:** Para sair digite `exit`.

```linux
ssh bandit0@bandit.labs.overthewire.org -p 2220
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes

bandit0@bandit.labs.overthewire.org's password: bandit0
```

Após login bem-sucedido, aparecerá um texto de boas vindas e outras informações

```linux
Linux bandit.otw.local 5.4.8 x86_64 GNU/Linux

      ,----..            ,----,          .---.
     /   /   \         ,/   .`|         /. ./|
    /   .     :      ,`   .'  :     .--'.  ' ;
   .   /   ;.  \   ;    ;     /    /__./ \ : |
  .   ;   /  ` ; .'___,/    ,' .--'.  '   \' .
  ;   |  ; \ ; | |    :     | /___/ \ |    ' '
  |   :  | ; | ' ;    |.';  ; ;   \  \;      :
  .   |  ' ' ' : `----'  |  |  \   ;  `      |
  '   ;  \; /  |     '   :  ;   .   \    .\  ;
   \   \  ',  /      |   |  '    \   \   ' \ |
    ;   :    /       '   :  |     :   '  |--"
     \   \ .'        ;   |.'       \   \ ;
  www. `---` ver     '---' he       '---" ire.org


Welcome to OverTheWire!
```
### Para Usuários Windows

Será necessario baixar um cliente ssh [openssh-cliente para windows](
https://tecnoblog.net/229971/windows-10-ativar-openssh-cliente/)
