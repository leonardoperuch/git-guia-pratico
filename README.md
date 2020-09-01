## Guia prático de uso do GIT E GITHUB


### Como instalar o GIT?
https://git-scm.com/book/pt-br/v2/Come%C3%A7ando-Instalando-o-Git

### Instalação do Editor - VSCODE
https://code.visualstudio.com/

### Repositório Remoto
http://github.com/

## CLient para GIT - Windows Shell
https://tortoisegit.org/


# AGENDA DO CURSO

- [X] Configurações iniciais

- [X] Inicializando seu projeto com GIT - Criando um repositório local GIT (diretório .GIT)

- [X] Criar um ponto na história da produção do seu projeto
- [x] Visualizar os pontos na linha do tempo

- [X] Visualizar o estado dos seus objetos que estão no seu diretório de trabalho
- [X] Visualizar o conteúdo dos seus objetos em um determinado ponto na linha do tempo

- [X] Criar uma nova versão do seu projeto, mas sem afetar os arquivos dessa linha do tempo principal.
- [X] Realizar alterações nessa nova versão.

- [X] Você adiciona as novas funcionalidades ao seu projeto em produção
- [X] Você quer deletar a branch da nova funcionalidade, depois de aplicar em seu projeto.

- [X] Adicionar seu projeto na nuvem (https://github.com/)
- [X] Realizar alterações locais e subir para a nuvem
- [X] Simular outras pessoas alterando o repositório remoto e seu repositório então tem que ser atualizado com as ultimas modificações
- [X] Resolver conflito em alterações do mesmo arquivo.

- [X] Começar a trabalhar em um outro projeto de alguém.

- [X] Git bash


# Principais comandos GIT

* `git config` // realiza as configurações iniciais
    * `git config --global user.name "Leonardo Peruch"` // Define a propriedade user.name
    * `git config --global user.email seuemail@exemplo.com` // Define a propriedade user.email
    * `git config --global core.editor code` // Define o seu editor principal
    * `git config user.name` // Exibe o valor da propriedade user.email
    * `git config user.email` // Exibe o valor da propriedade user.email
    * `git config --list` // Exibe o valor de todas as propriedades

* `git init` // inicia um repositório do GIT a partir do diretório corrente. 

* `git add` // envia mudanças para área de preparação
    * `git add <nome_arquivo>` // adiciona um arquivo específico
    * `git add .` // adiciona vários arquivos

* `git commit` // adiciona um ponto na linha do tempo
    * `git commit -m 'seu comentario sobre a alteracao'` // Faz o commit dos arquivos para o repositório git
    * `git commit -am 'seu comentario sobre a alteracao'` // Adiciona (add) e faz o commit em um unico comando

* `git log` // visualiza os pontos na linha do tempo / commit
    * `git log --oneline --graph` // Visualiza os commit em modo linear e como um grafo

* `git status` // informa o estado das alterações do projeto

* `git show` // apresenta determinado ponto na história
    * `git show <cod_commit>` // Visualiza um determinado ponto na historia
    * `git show` // Visualiza o último ponto na história

* `git branch` // gerenciar novas ramificações da linhas do tempo
    * `git branch <nome_do_branch>` // Cria uma nova ramificação
    * `git branch` // Visualiza as linhas do tempo
    * `git branch -D <nome_do_branch>` // Deleta uma ramificação

* `git checkout` // manipula as linhas do tempo
    * `git checkout <nome_do_branch>` // Baixa algum branch específico
    * `git checkout <nome_do_arquivo>` // Baixa somente o arquivo
    * `git checkout -B <nome_do_branch>` // Cria uma nova ramificação e já faz o checkout

* `git merge` // unir linhas do tempo
    * `git merge <nome_do_branch>`

# Principais comandos GIT para trabalhar com o repositório remoto

* `git remote add origin <url_site>` // comandos para gerenciar o repositório remoto
    * `git remote add origin <url_site>` // associa o repositório local com o repositório remoto da url

* `git push` // envia alterações locais para o repositório remoto
    * `git push -u origin master` 

* `git pull` //  atualizar o repositório local com arquivos remotos diferentes

* `git clone` // clonar um projeto / repositório
    * `git clone https://github.com/leonardoperuch/git-guia-pratico`

