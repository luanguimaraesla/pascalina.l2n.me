+++
title = "Criando um site do zero"
description = ""
type = ["posts","post"]
tags = [
    "golang",
    "hugo",
    "site"
]

date = "2020-08-02"

categories = [
    "development",
    "website",
]

series = ["Tutoriais"]

[ author ]
  name = "Mariana Fonseca"
+++

Nós decidimos começar este site para podermos compartilhar coisas interessantes que lemos, estudamos, os desafios que temos encontrado. Além disso, também pensamos em um espaço para comentarmos sobre documentários, filmes, livros, personalidades que nos inspiram nesse projeto. 

Para isso, nos propusemos a aprender como fazer o nosso próprio site! Vamos colocar aqui um passo-a-passo de como fizemos.

Primeiramente, instalamos e iniciamos o Git nos nossos computadores. O Git é um gerenciador de versões, muito útil para controlarmos melhor as alterações que fazemos em documentos e repositórios. Como este é um site colaborativo, fica muito mais fácil! 

Depois de instalar o Git no computador (talvez já tenha uma versão instalada, confere digitando `git --version` no terminal), criamos uma pasta para armenzar as informações do projeto e então percorremos os seguintes passos sempre usando o terminal:

```bash
  # executamos este comando dentro da pasta 
  # onde salvamos nosso site
  git init 

  # com este comando vemos as alterações
  # que precisamos salvar
  git status 

  # adicionamos todas as alterações realizadas
  # ao próximo commit
  git add -A 
  
  # criamos um commit com as alterações. esse passo  
  # é muito importante para lembrarmos o que
  # significa cada alteração que fizemos em
  # cada versão. use mensagens significativas.
  git commit -m "mensagem de identificação" 
  
  # vemos todas edições feitas com este comando
  git log 
```

Depois de criada a nossa pasta, escolhemos um tema para a estrutura básica do nosso site. Existem várias maneiras de criar o seu próprio site (ferramentas como Wordpress, Wix), mas, como este é um projeto de programação, optamos por uma ferramenta mais simples que usa a programação na criação de sites.

O [Hugo](https://gohugo.io) é uma ferramenta desenvolvida em Golang que possibilita a criação de sites estáticos de uma maneira fácil e intuitiva. Por isso também instalamos o Hugo para iniciar o nosso site. Como já temos o Homebrew instalado:

```bash
  brew install hugo
```

Depois de instalado, nós selecionamos um tema que representasse bem a nós 7 e ao nosso projeto e pedimos para o Hugo criar nosso site (; - dentro da pasta do nosso projeto!:

```bash
  hugo new site pascalina
```
 
Com isso o Hugo cria uma nova pasta com as informações do nosso site. Nessa pasta nós inserimos o código do tema que selecionamos anteriormente:

```bash
  git clone <link_do_hugo_com_o_codigo_do_tema_escolhido>
```

Esses dados são super importantes, então já salvamos tudo com o Git, seguindo os mesmos passos dali de cima. Em seguida para fazermos a personalização do nosso site, nós usamos nosso editor de código: 

```bash
  code .
```

Copiamos a estrutura básica, que já vem com o código do tema que selecionamos no Hugo (geralmente essa informação vem em uma pasta chamada `exampleSite`), e o inserimos no arquivo `config.toml`, que já está também na pasta com as informações do nosso site. 

A partir daí fizemos as alterações e personalizamos o nosso site como preferimos! Para executarmos o site e vermos como estava ficando usamos: 

```bash  
  hugo server -D
```

Depois, nós salvamos tudo de novo com Git. Mas para não correr o risco de perder todo nosso trabalho e também para facilitar o compartilhamento dos dados do nosso site, utilizamos o GitHub para salvar tudo. 

Depois de criar e configurar a nossa conta, basta criar um repositório do GitHub para armazenarmos os dados, criamos um repositório também chamado pascalina! Para inserir as informações do nosso computador no GitHub é muito simples: 

```bash
  git remote add origin <link_do_repositorio_no_GitHub>

  git push origin master
```

Nós sempre salvamos as nossas alterações no GitHub. Em outro post nós explicamos como contribuímos em projetos no GitHub e a construção deste site foi nosso primeiro projeto colaborativo! 
