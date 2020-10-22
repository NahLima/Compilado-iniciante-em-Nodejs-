## Aqui vamos encontrar um guia prático pra quem está começando no universo da programação! 


![112-installing](../img/112-installing.png)

| *Alguns temas abordados:*
|-------------------------|
| Front-end e Back-end|
| Banco de dados 
| Acessando o seu terminal 
| Git e GitHub
|Lógica de programação com JavaScript/Nodejs
|Api
| Auntentificação


## Front-end
Desenvolvimento web front-end é a prática de converter dados em uma interface gráfica, através do uso de HTML, CSS e JavaScript, para que os usuários possam visualizar e interagir com esses dados. É a área responsável por desenvolver a parte relacionada ao layout, mas não é só isso, o front-end também trabalha com lógica.

| *Principais ferramentas:* 
|---------------------------|
|HTML
|CSS
|JavaScript
|React

## Back-end 
Back-end é a parte da aplicação que faz o tratamento de dados e a comunicação com o banco de dados. Quando acessamos um site, por exemplo, por trás de toda sua apresentação amigável esteticamente, há uma comunicação das informações trocadas entre banco de dados e navegador. Portanto, por trás da interface gráfica do realizador, o back-end está sempre agindo, ou seja, tudo que dá estrutura e apoio às ações do usuário da máquina é chamado de back-end.

| *Principais linguagens usadas:*
|---------------------------------|
| Java
| PHP
| Ruby
| Javascript ( Node)
| C#
| Python


## Banco de dados

Banco de dados de forma mais simples, é o agrupamento de dados que tratam do mesmo assunto, e que precisam ser armazenados para segurança ou conferência futura. 

É comum que empresas tenham diversas informações que precisam ser organizadas e disponibilizadas dentro do negócio para que sejam consultadas posteriormente pela equipe e pela gerência.

Podemos adicionar dados, editar, excluir e modificar em um banco de dados.

|*Os mais usados são:*
|---------------------------------|
|MYSQL --> relacional
|PostgreSQL -->  relacional
|MongoDB --> orientado a documentos
|Redis

## Acessando o terminal do computador

![terminal](https://camo.githubusercontent.com/f41ac57d05a14def0daf72fd049ac9ab01ee8bc2/68747470733a2f2f7777772e6c756361736361746f6e2e636f6d2e62722f6173736574732f696d616765732f323031382f30312f7465726d696e616c2d77696e646f77732e706e67)

Através do terminal que podemos dar comandos ao computador, os comandos básicos são:

**dir** (windows)

**Ls ou list**  listar arquivos, mostra tudo o que vc tem no pc

**ls** - para listar os arquivos e pastas dentro de um diretório

**cd nome-da-pasta**  para navegar entre diretórios

**cd ..**  sair de um diretório

**mkdir nome-da-pasta**  cria uma pasta

**touch nome-do-arquivo**  cria um arquivo

**del nome-do-arquivo (windows) / rm nome-do-arquivo** deleta um arquivo

**rd nome-da-pasta (windows) / rmkdir nome-da-pasta**  exclui um diretório

**cls (windows) /clear**  limpa o terminal

**F7 (windows) / history**  mostra o histórico de comandos

**tree**  podemos ver a árvore de diretórios do nosso sistema de uma forma mais gráfica

:+1: Se usarmos o Git Bash os atalhos "ficam universais" assim você não precisa ter de lembrar todos os comandos para cada tipo de sistema. 


## Git e GitHub

### Git 

![GitHub Logo](https://media.giphy.com/media/kH6CqYiquZawmU1HI6/giphy.gif)

O **Git** é um sistema de controle de versão que, pela sua estrutura interna, é
umamáquina do tempo extremamente rápida e é um robô de integração bem
competente.
Foi criado em 2005 por _Linus Torvalds_, o mesmo criador do Linux, que
estava descontente como BitKeeper, o sistema de controle de versão utilizado
no desenvolvimento do kernel do Linux.
Hoje em dia, além do kernel do Linux, a ferramenta é utilizada em diversos
outros projetos de código aberto. O Git também é bastante utilizado em
empresas em todo o mundo, inclusive no Brasil.
Atualmente, conhecer bem como utilizar o Git é uma habilidade importante
para uma carreira bem-sucedida no desenvolvimento de software.

### Instalação do Git
O git já vem instalado na maioria dos computadores Mac e Linux, se for o seu, apenas digite na linha de comando: git --version caso esteja instalado, esse comando mostrará a versão do git.

tutorial: https://woliveiras.com.br/posts/instalando-o-git-windows/

git para mac: https://git-scm.com/download/mac
git para windows: https://gitforwindows.org/
git para plataformas Linux/Debian, como o Ubuntu: digite na linha de comando _sudo apt-get install git_


### Git configuração
Para adicionar usuário:

git config --global user.name "fulano"
git config --global user.email “fulano@hotmail.com”
Para remover usuário:

git config --global --unset user.name "fulano"
git config --global --unset user.email “fulano@hotmail.com”



## GitHub
![GitHub Logo](https://media.giphy.com/media/du3J3cXyzhj75IOgvA/giphy.gif)

**GitHub** é uma plataforma de hospedagem de código-fonte com controle de versão usando o Git. Ele permite que qualquer usuário cadastrado na plataforma hospede seu código e contribua em projetos.

### Criando conta no GitHub
Acesse o link : [GitHub](http://github.com).

### Iniciando um projeto com Git

- No terminal dentro da pasta que vai conter todos os arquivos do seu projeto dê o comando ``git init``, com ele o git vai criar uma pasta oculta com o nome .git.
- Com o comando ``git status`` conseguimos ver o status do repositório que de início é ‘Untracked files’, esse status diz que não tem nenhum arquivo para ser rastreado ( para criar versões ).
- Para o arquivo ser rastreado usamos o comando ``git add nome-do-arquivo`` ou se desejar ``git add .`` que vai adicionar todos os arquivos de uma vez.
- Se dermos um ``git status`` novamente o status vai ser ‘Changes to be committed’, isso quer dizer que o arquivo pode ganhar uma versão.
- ``git commit -m “mensagem do commit” `` é o comando que rodamos para o projeto ganhar uma nova versão.
- ``git log `` é o comando que imprime todo o histórico de commits dados no projeto.


### Repositório remoto

- Primeiro iniciamos o repositório com ``git init, git add . , git commit`` 
- Criamos um repositorio no github 
- ``git remote add origin url-que-voces-copiaram-do-github`` conectamos aquele repositório local com um remoto
-``git push origin master`` é o comando que damos pra subir as alterações que fizemos no projeto para o github.

``git status`` Esse comando nos ajuda a ver os estágios dos arquivos. Antes do add e do commit podemos usá-lo para ver quais arquivos foram criados e ou modificados.

##### Files stages (Estágios do arquivo)

**untracked files** não deu instrução ao git do que fazer com o arquivo
**changes to be committed** adicionou, mas não deu o commit
**commited** commit foi feito


### Clone

Para trazer uma cópia de um repositório remoto para o seu computador usamos:

`` git clone ulr-do-repo-no-github ``

Usamos o comando ``git pull`` para atualizar nossa repositório local com o remoto.


### Branch

Branch são ramificações dentro do seu projeto, ou seja, uma branch é uma linha independente de desenvolvimento em que podemos comitar novas versões do código sem afetar o projeto.
![GitHub Logo](https://raw.githubusercontent.com/reprograma/on7-porto-s1-introducao/master/images/branch.png)

- ``git checkout -b nome-da-branch `` para criar uma branch
- `` git branch`` para visualizar as branchs existentes
- ``git checkout nome-da-branch`` para trocar de branch
- `` git merge nome-da-branch`` é o comando que uso para trazer as modificações de uma branch para outra. 

### Pull Request - PR

É através de pull request que podemos contribuir com outros projetos, e fica em responsabilidade do dono do repositório autorizar o merge da suas alterações, podendo ele negar, pedir correções entre outras coisas.
- Fork o repositório no github 
- Clonar repositório (git clone url-do-projeto)
- Criar sua branch para trabalhar git checkout -b nome-da-sua-branch

- Faça mudanças e: 
  - git add .
  - git commit -m "o que eu fiz"
  - git push origin nome-da-sua-branch
- Agora vamos no github abrir a PR  :octocat: 


### Readme.md MARKDOWN
Arquivo essencial para todo repositório no github. onde explicamos o projeto e damos algumas instruções, caso necessário.

https://dillinger.io/

https://guides.github.com/pdfs/markdown-cheatsheet-online.pdf

### links úteis:
https://medium.com/reprogramabr/git-e-github-por-onde-come%C3%A7ar-ca88a783c223 -> Medium Reprograma. Escrito por Thaylla <3

https://git-scm.com/book/pt-br/v1/Primeiros-passos-Sobre-Controle-de-Vers%C3%A3o -> Documentação oficial do git em português.

https://rogerdudler.github.io/git-guide/index.pt_BR.html -> git - guia prático


Obrigada! 

