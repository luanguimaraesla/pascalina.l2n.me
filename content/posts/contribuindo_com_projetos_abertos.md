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

Para essa receita você vai precisar de: acesso a internet, uma conta no GitHub, ter o Git instalado no seu computador ([confere aqui](https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Instalando-o-Git)), criatividade para colaborar com projetos e uma pitada de curiosidade.
   
**_Tá a fim de compartilhar conhecimento? Então vem!_**

![gif](https://media.giphy.com/media/NXp9HM6YeuS0U/giphy.gif)

Contribuir com um projeto aberto utilizando as ferramentas que vamos detalhar melhor nesse post, é tipo isso mesmo, uma receitinha de bolo.

Vamos adotar como exemplo para essa explicação, a forma como nos colaboramos para construção desse site, o Pascalina <3

1. Primeiro, você precisa criar uma conta no GitHub, uma plataforma de hospedagem de código-fonte com controle de versão usando o Git. Essa ferramenta possibilita que programadores, utilitários ou qualquer usuário cadastrado contribuam com projetos abertos ou privados de qualquer lugar do mundo ([1](https://pt.wikipedia.org/wiki/GitHub)).

2. Depois encontre o diretório do projeto dentro do GitHub. No nosso caso, o diretório do projeto pode ser acessado por esse link: <https://github.com/luanguimaraesla/pascalina>. Dê uma olhada e veja como é organizado um diretório, o site disponibiliza uma série de ferramentas para trabalharmos.

3. Agora é necessário que você faça um Fork do repositório onde se encontra o projeto do seu interesse. Essa função permite a criação de uma cópia de um repositório, onde é possível experimentar livremente alterações sem afetar o projeto original ([2](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo)).

   Para isso, basta clicar no botão “Fork” localizado no canto superior direito, como mostra a imagem a seguir. Quando o Fork do repositório for concluído, você será redirecionado automaticamente para a cópia do repositório na sua conta do GitHub.

![Legenda](/fork.png) 

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

7. [To do]


#### Referências

(1) GitHub. Disponível em: <https://pt.wikipedia.org/wiki/GitHub> \
(2) Fork a repo. Disponível em: <https://docs.github.com/en/github/getting-started-with-github/fork-a-repo> \
(3) Markdown. Disponível em: <https://pt.wikipedia.org/wiki/Markdown> \
(4) Markdown guide. Disponível em: <https://www.markdownguide.org/basic-syntax/>