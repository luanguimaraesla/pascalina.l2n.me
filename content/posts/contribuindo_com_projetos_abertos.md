+++
title = "Como contribuir com projetos abertos"
description = "Um tutorial simples de como contribuir com projetos abertos utilizando o GitHub"
type = ["posts","post"]
tags = [
    "opensource",
    "free",
    "freesoftware",
    "github",
]

date = "2020-08-03"

categories = [
    "Contribution",
    "opensource",
]

series = ["Tutoriais"]

[ author ]
  name = "Tainara Costa"
+++

Para essa receita você vai precisar de: acesso à internet, uma conta no GitHub, ter o Git instalado no seu computador ([saiba mais aqui](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Instalando-o-Git)), criatividade para colaborar com projetos e uma pitada de curiosidade.
   
**_Tá a fim de compartilhar conhecimento? Então vem!_**

![gif](https://media.giphy.com/media/NXp9HM6YeuS0U/giphy.gif)

Contribuir com um projeto aberto utilizando as ferramentas que vamos detalhar melhor nesse post, é tipo isso mesmo, uma receitinha de bolo.

Vamos adotar como exemplo para essa explicação, a forma como nos colaboramos para construção desse site, o Pascalina <3

> Vale lembrar que o nosso site foi feito utilizando o Hugo, que é um gerador de sites estáticos, desenvolvido em Golang. É uma aplicação que auxilia o usuário a gerenciar, publicar e divulgar o seu conteúdo de uma maneira mais rápida e prática. Leia mais sobre o Hugo e a sua instalação [(aqui](https://gohugo.io/about/)).

1. Primeiro, você precisa criar uma conta no GitHub, uma plataforma de hospedagem de código-fonte com controle de versão usando o Git. Essa ferramenta possibilita que programadores, utilitários ou qualquer usuário cadastrado contribuam com projetos abertos ou privados de qualquer lugar do mundo ([1](https://pt.wikipedia.org/wiki/GitHub)).

2. Depois encontre o diretório do projeto dentro do GitHub. No nosso caso, o diretório do projeto pode ser acessado por esse link: <https://github.com/luanguimaraesla/pascalina>. Dê uma olhada e veja como é organizado um diretório, o site disponibiliza uma série de ferramentas para trabalharmos.

3. Agora é necessário que você faça um Fork do repositório onde se encontra o projeto do seu interesse. Essa função permite a criação de uma cópia de um repositório, onde é possível experimentar livremente alterações sem afetar o projeto original ([2](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo)).

Para isso, basta clicar no botão “Fork” localizado no canto superior direito, como mostra a imagem a seguir. Quando o Fork do repositório for concluído, você será redirecionado automaticamente para a cópia do repositório na sua conta do GitHub.

![Fork](/fork.png) 

4. Agora vamos iniciar o acesso para inserir nossas contribuições. No canto superior direito podemos encontrar o botão “Code”, como mostra a imagem. Ao clicar nele, será exibida uma caixa com um link URL, copie esse link.

![Code](/code.png)

5. Abra o terminal do seu computador e altere o diretório de trabalho atual para o local em que deseja ter o diretório clonado. Depois execute o seguinte comando:

```
$ git clone [cole o link aqui]

```

6. Pronto! A pasta do repositório agora está salva no seu computador. Abra a mesma no seu editor de código para ter acesso as pastas e códigos do repositório que foi copiado. Lembrando que toda alteração feita nesse projeto não irá afetar o código original.

No nosso exemplo, estamos contribuindo para a publicação de um post no site Pascalina, mas você pode usar esse tutorial para realizar outros tipos de alterações.

Provavelmente, no seu editor de código você poderá navegar pelas pastas que estão na raiz do projeto e inserir suas modificações no código. Nesse caso, a criação de posts é feita acessando as pastas: Content > Posts. Dentro da pasta “Post” você criará um documento com a extensão _.md_ e poderá escrever o texto que pretende publicar no site, para isso usamos uma linguagem específica no nosso projeto, chamada _Markdown_.

> Markdown é uma linguagem simples de marcação, originalmente criada por John Gruber e Aaron Swartz, ela converte seu texto em HTML válido ([3](https://pt.wikipedia.org/wiki/Markdown)).\
> Leia um pouco mais sobre como usar essa linguagem no Markdown Guide ([4](https://www.markdownguide.org/basic-syntax/)).

7. Quando você encerrar e salvar todas as contribuições que desejava fazer no código do projeto, é necessário enviá-las para o GitHub para que de fato elas sejam implementadas e a contribuição seja feita. Esse processo é realizado por meio do Git, precisaremos rodar alguns comandos no nosso terminal (certifique-se que o diretório atual seja o do projeto).

O primeiro comando dessa etapa é o hugo, ele gera seu site no diretório público e assim está tudo pronto para ser implantado no seu servidor da web ([5](https://gohugo.io/getting-started/usage/)).

```
$ hugo
```

Em seguida, podemos observar todas as mudanças feitas e arquivos criados, com o comando:

```
$ git status
```
O resultado desse comando é uma série de mudanças implementadas por nós e pelo Hugo automaticamente. Para adicionar todas essas mudanças na área de _stage_, usamos o comando:

```
$ git add -A
```

Agora vamos salvar essas mudanças com o comando:

```
$ git commit -m “adding a new post - how to contribute to open source projects”
```

Entre as aspas você pode inserir qualquer comentário que te ajude a identificar esse commit caso seja necessário.

E para passar todas essas mudanças do repositório local, ou seja, do seu computador para o repositório remoto que é o GitHub, usamos o comando:

```
$ git push origin master
```

Assim, todas as mudanças que você realizou no projeto estão agora salvas no GitHub.

8. Para que as contribuições sejam aceitas pelo autor do projeto o qual você está sugerindo mudanças, é preciso fazer um pedido para que ele as aceite. Esse pedido é feito por meio do _pull request_, para acessar essa função devemos voltar ao repositório origem do projeto e clicar na aba “Pull requists”, como mostra a imagem.

![](/pull_requests.png)

Dentro dessa aba você irá clicar no botão “New pull requist”.

![](/new_pull_request.png)

E então irá aparecer a página de Compare changes, uma forma do GitHub certificar que a inserção das suas mudanças não irão danificar o código origem. Para fazer a comparação entre seu código e o código origem clique na opção “compare across forks” e mude o “head repository” para o seu repositório, essa opção vai estar disponível na lista quanto clicar no botão dessa ferramenta. Se tudo estiver ok, vai aparacer a seguinte mensagem “Able to merge” e assim você poderá clicar no botão “Create pull request”. Esse passo pode ser observado na imagem abaixo:

![](/compare.png)

9. Em seguida irá aparecer a página de Open a pull request, onde você pode enviar uma mensagem junto com as modificações explicando para o autor do projeto o objetivo e os detalhes da sua colaboração. Por fim, clique no botão “Create pull request”

![](/create.png)

**E pronto!** Sua colaboração foi enviada e estará disponível para o autor conferir e decidir se irá aceitá-la.

_Agora, sabendo como enviar sua colaboração para um projeto open source, fique a vontade para colaborar com o Pascalina!_


#### Referências

(1) GitHub. Disponível em: <https://pt.wikipedia.org/wiki/GitHub> \
(2) Fork a repo. Disponível em: <https://docs.github.com/en/github/getting-started-with-github/fork-a-repo> \
(3) Markdown. Disponível em: <https://pt.wikipedia.org/wiki/Markdown> \
(4) Markdown guide. Disponível em: <https://www.markdownguide.org/basic-syntax/> \
(5) Basic Usage – Hugo. Disponível em: <https://gohugo.io/getting-started/usage/>

