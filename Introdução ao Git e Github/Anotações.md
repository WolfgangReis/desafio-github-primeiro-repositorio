# ANOTAÇÕES :pencil:

Este material contém algumas anotações com passo a passo de como criar um repositório no Github.

[Download do Git](https://git-scm.com/download)

### Abrindo o Git Bash

O **Git Bash** é o terminal através do qual será possível utilizar as funções do Git. Para abri-lo, basta clicar com o botão direito d mouse em alguma pasta, ou mesmo na área de trabalho, e selecionar a opção **Git Bash Here**. Aparecerá uma janela com esta abaixo.

![Console Git](https://github.com/WolfgangReis/desafio-github-primeiro-repositorio/blob/main/Introdu%C3%A7%C3%A3o%20ao%20Git%20e%20Github/Imagens/Console%20Git.JPG?raw=true)



### Crie seu repositório no Github

Primeiramente, é necessário ter uma [conta no Github](https://github.com/). Depois de cadastrado, procure pela aba **Repositórios** na sua página de perfil. Nesta página, selecione "New".

![New1](https://github.com/WolfgangReis/desafio-github-primeiro-repositorio/blob/main/Introdu%C3%A7%C3%A3o%20ao%20Git%20e%20Github/Imagens/new1.JPG?raw=true)



Assim, você será redirecionado para uma nova página onde escolherá o nome do repositório e uma descrição para ele (se quiser).

![New2](https://github.com/WolfgangReis/desafio-github-primeiro-repositorio/blob/main/Introdu%C3%A7%C3%A3o%20ao%20Git%20e%20Github/Imagens/new2.JPG?raw=true)

Aqui você pode também selecionar a opção de criar um arquivo **README.md **, que é um arquivo de texto onde você pode colocar algumas informações sobre seu repositório. Depois clique em **Create repository** e pronto! Estará criado seu repositório no Github!

![New3](https://github.com/WolfgangReis/desafio-github-primeiro-repositorio/blob/main/Introdu%C3%A7%C3%A3o%20ao%20Git%20e%20Github/Imagens/new3.JPG?raw=true)

### Acessando o repositório pelo Git

Depois de criado o repositório, acesse o repositório no seu perfil do Github e clone o repositório.

![copiando chave do repositório](https://github.com/WolfgangReis/desafio-github-primeiro-repositorio/blob/main/Introdu%C3%A7%C3%A3o%20ao%20Git%20e%20Github/Imagens/clone1.JPG?raw=true)

Copiada a chave, vá ao **Git Bash** aberto na página desejada e digite o comando ***git clone*** seguido do link que você acabou de copiar. Aperte a tecla **Enter**.

![clonando](https://github.com/WolfgangReis/desafio-github-primeiro-repositorio/blob/main/Introdu%C3%A7%C3%A3o%20ao%20Git%20e%20Github/Imagens/clonando.jpg?raw=true)

Com isso, um novo diretório será criado em sua máquina. Você pode acessá-lo utilizando o comando ***cd*** seguido do nome do repositório.

![abrindo diretório do novo repositório](https://github.com/WolfgangReis/desafio-github-primeiro-repositorio/blob/main/Introdu%C3%A7%C3%A3o%20ao%20Git%20e%20Github/Imagens/abrindo%20dir.jpg?raw=true)

Já dentro da sua pasta do repositório, é possível verificar o status da pasta através do comando ***git status***, ele indica se falta algo a ser feito (push, commit, etc) ou se está tudo em ordem.

![abrindo diretório do novo repositório](https://github.com/WolfgangReis/desafio-github-primeiro-repositorio/blob/main/Introdu%C3%A7%C3%A3o%20ao%20Git%20e%20Github/Imagens/abrindo%20dir2.jpg?raw=true)

### Enviando seu arquivo do pc para o Github

Foi criada uma pasta dentro do diretório no computador.

![Pasta de exemplo criada](https://github.com/WolfgangReis/desafio-github-primeiro-repositorio/blob/main/Introdu%C3%A7%C3%A3o%20ao%20Git%20e%20Github/Imagens/pasta%20exemplo.jpg?raw=true)

Foi criado um arquivo de texto dentro da *Pasta de anotações*.

![arquivo txt criado dentro da pasta de anotações](https://github.com/WolfgangReis/desafio-github-primeiro-repositorio/blob/main/Introdu%C3%A7%C3%A3o%20ao%20Git%20e%20Github/Imagens/pasta%20exemplo2.jpg?raw=true)

Esta pasta e este arquivo foram criados apenas para exemplificar o que ocorre quando há uma alteração da pasta que foi clonada do Github.

Agora, ao digitar o comando ***git status***, o Git Bash acusa alguns arquivos que estão *untracked*. Isto significa que ainda não foram modificados no Github, apenas no seu computador local.

![status de untracked](https://github.com/WolfgangReis/desafio-github-primeiro-repositorio/blob/main/Introdu%C3%A7%C3%A3o%20ao%20Git%20e%20Github/Imagens/status%20untracked.jpg?raw=true)

Para que o Git entenda que o arquivo foi modificado e deve ser adicionado ao Github, usa-se o comando ***git add .***. Desta forma, ao usar o ***git status***, pode-se verificar que a mudança foi feita.

![adicionando e verificando as alterações](https://github.com/WolfgangReis/desafio-github-primeiro-repositorio/blob/main/Introdu%C3%A7%C3%A3o%20ao%20Git%20e%20Github/Imagens/adicionando.jpg?raw=true)

Lembrando que estas alterações foram adicionada apenas localmente. Ainda precisamos dar um commit para que o Git entenda que as alterações desejadas já foram feitas antes de enviar para o Github de forma remota.

O commit se dá através do comando ***git commit***. Após a alteração é comum colocar uma mensagem indicando qual foi a alteração realizada. Esta é uma boa prática e ajuda a entender a alteração caso sejam feitas consultas futuramente. Para deixar uma mensagem, usa-se o comando ***git commit -m "Sua mensagem aqui"***.

![dando commit nas alterações](https://github.com/WolfgangReis/desafio-github-primeiro-repositorio/blob/main/Introdu%C3%A7%C3%A3o%20ao%20Git%20e%20Github/Imagens/commit.jpg?raw=true)

Verifica-se então como está o status do repositório e nota-se que está tudo limpo, falta apenas usar o *push*.

![status após o commit](https://github.com/WolfgangReis/desafio-github-primeiro-repositorio/blob/main/Introdu%C3%A7%C3%A3o%20ao%20Git%20e%20Github/Imagens/commit2.jpg?raw=true)

Agora iremos enfim enviar o repositório para o Github. Faremos isso através do comando ***git push origin main***.

![enviando para o Github](https://github.com/WolfgangReis/desafio-github-primeiro-repositorio/blob/main/Introdu%C3%A7%C3%A3o%20ao%20Git%20e%20Github/Imagens/push.jpg?raw=true)

Verificamos novamente o status.

![status depois do push](https://github.com/WolfgangReis/desafio-github-primeiro-repositorio/blob/main/Introdu%C3%A7%C3%A3o%20ao%20Git%20e%20Github/Imagens/push2.jpg?raw=true)

Pronto! Agora seu repositório está atualizado no seu perfil do Github com todas as alterações que foram feitas. A nova pasta e o novo arquivo de texto.

![repositório Github depois da atualização](https://github.com/WolfgangReis/desafio-github-primeiro-repositorio/blob/main/Introdu%C3%A7%C3%A3o%20ao%20Git%20e%20Github/Imagens/push3.jpg?raw=true)

### Alguns comandos úteis para se usar no Git Bash

- Limpar os comandos anteriores da tela: **CTRL + L**
- Criar um novo diretório: ***mkdir***
- Remover um diretório: ***rmdir***
- Exibir o caminho do diretório atual: ***pwd***
- Listar o conteúdo do diretório atual: ***ls***
- Mudar de diretório: ***cd***
- Iniciando um repositório local: ***git init***
- Verificando status dos arquivos: ***git status***
- Enviando todos os arquivos para o Stage: ***git add .*** ou ***git add -a***
- Enviando o que está no Stage para o HEAD: ***git commit -m "titulo do commit"***
- Adicionando e indicando a URL em que serão mantidos os arquivos no repositório remoto: ***git remote add origin URLdoRepositorio***
- Enviando arquivos para o repositório especificado: ***git push origin main*** ou ***git push origin master***

#### Mais comandos do Git podem ser obtidos nos links abaixo

[Comandos do Git leocomelli](https://gist.github.com/leocomelli/2545add34e4fec21ec16)

[Comandos do Git](https://comandosgit.github.io/)
