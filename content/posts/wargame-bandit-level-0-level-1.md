---
title: "WarGame Bandit Level 0 - Level 1"
date: 2021-09-27T22:20:15-03:00
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
description: "Desc Text."
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

https://overthewire.org/wargames/bandit/bandit1.html


## Meta

>The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

## Possíveis comandos para resolver o problema

> ls, cd, cat, file, du, find

https://explainshell.com/

* **ls** lista arquivos é diretórios.
* **cd** usado para navegar entre diretorios.
   
    Para entrar em um diretório digite `cd NomePasta`, voltar um diretorio use `cd ..`
* **cat** imprime o conteúdo do arquivo.
* **file** informa o tipo do arquivo. 
* **du** exibe informaçõe sobre o espaço ocupado.
* **find** pesquisa o nome do arquivo dentro do diretório.

## Write up

### Conectando 
* Nome do host: `bandit.labs.overthewire.org`
* Nome do usuario: `bandit0`
* Senha: `bandit0`
* Porta: `2220`

**Passo 1:** Após conectarmos, estaremos no diretorio inicial digite o comando `ls`, que mostrar o conteudo deo diretório o arquivo `readme`.

**Passo 2:** Digite o comando `cat` e o nome do arquivo.

**Passo 3:** Para sair digite `exit`.
   
### Solução 

```linux
$ ssh bandit0@bandit.labs.overthewire.org -p 2220

bandit0@bandit:~$ ls
readme

bandit0bandit:~$ cat readme
boJ9jbbUNNfktd78OOpsqOltutMc3MY1

bandit0@bandit:~$ exit
logout
Connection to bandit.labs.overthewire.org closed.
```
## Level 1

* Username: `bandit1`
* Password: `boJ9jbbUNNfktd78OOpsqOltutMc3MY1`