## <h2 style="display: flex; align-items: center;"><img src="https://play-lh.googleusercontent.com/PCpXdqvUWfCW1mXhH1Y_98yBpgsWxuTSTofy3NGMo9yBTATDyzVkqU580bfSln50bFU" width="60" height="60" style="margin-left: 10px;"> Módulo 1 </h2>




## Sumário
1. [Introdução](#introdução)
2. [Comandos Básicos](#comandos-básicos)
  - [git init](#git-init)
  - [git remote](#git-remote)
  - [git add](#git-add)
  - [git add .](#git-add-)
  - [git status](#git-status)
  - [git commit](#git-commit)
  - [git push](#git-push)
  - [git pull](#git-pull)
3. [Comandos Úteis](#comandos-úteis)
  - [git clone](#git-clone)
  - [git log](#git-log)
  - [git branch](#git-branch)
  - [git checkout](#git-checkout)
  - [git merge](#git-merge)


## Introdução
Git é um sistema de controle de versão distribuído, criado por Linus Torvalds em 2005, que permite aos desenvolvedores rastrear mudanças no código-fonte durante o desenvolvimento de software. Ele ajuda a coordenar o trabalho entre várias pessoas e a registrar o histórico completo das alterações feitas em um projeto.


GitHub é uma plataforma de hospedagem de código-fonte e arquivos com controle de versão utilizando Git. Ele oferece uma interface web amigável para gerenciamento de repositórios Git, além de ferramentas para colaboração, revisão de código e integração contínua.


### O que é Controle de Versão?
Controle de versão é a prática de gerenciar e registrar alterações em arquivos ao longo do tempo. Ele permite que desenvolvedores trabalhem simultaneamente no mesmo projeto sem conflitos, rastreiem a origem das mudanças e revertam para versões anteriores quando necessário.


### Benefícios do Controle de Versão:
- **Colaboração**: Várias pessoas podem trabalhar no mesmo projeto simultaneamente.
- **Histórico**: Todas as alterações são registradas, permitindo reverter para versões anteriores.
- **Backups**: Código-fonte e arquivos são armazenados em locais remotos seguros.
- **Rastreabilidade**: Fácil identificação de quem fez quais alterações e por quê.




## Comandos Básicos
### git init
O comando `git init` é usado para criar um novo repositório Git. Este comando cria um diretório oculto chamado `.git`, onde todas as informações necessárias do repositório são armazenadas.


```sh
git init
```


### git remote
O comando git remote é usado para gerenciar os repositórios remotos. Por exemplo, para adicionar um repositório remoto chamado origin, usamos:


```sh
git remote add origin https://github.com/usuario/repositorio.git
```


### git add
O comando git add adiciona mudanças no diretório de trabalho para a área de stage. Para adicionar um arquivo específico, use:


```sh
git add nome_do_arquivo
```
### git add .
O comando git add . adiciona todas as mudanças no diretório de trabalho para a área de stage. Isso inclui novos arquivos, modificações em arquivos existentes e deleções.


```sh
git add .
```


### git status
O comando git status mostra o estado atual do diretório de trabalho e da área de stage. Ele exibe as mudanças que foram staged, as que não foram e arquivos que não estão sendo rastreados.


```sh
git status
```


### git commit
O comando git commit é usado para salvar as mudanças na história do repositório. Geralmente, adicionamos uma mensagem de commit descritiva usando a flag -m:


```sh
git commit -m "Mensagem do commit"
```


### git push
O comando git push é usado para enviar as mudanças do repositório local para um repositório remoto. Para enviar as mudanças para o repositório remoto origin no branch main, usamos:


```sh
git push origin main
ou
git push origin nome-da-branch
```


### git pull
O comando git pull é usado para buscar e integrar as mudanças de um repositório remoto para o branch atual.


```sh
git pull origin main
ou
git pull origin nome-da-branch
```


## Comandos Úteis


### git clone
O comando git clone é usado para criar uma cópia local de um repositório remoto. Isso é útil para começar a trabalhar em um projeto existente.


```sh
git clone https://github.com/usuario/repositorio.git
```
### git log
O comando git log exibe o histórico de commits do repositório. Ele mostra a lista de commits realizados, juntamente com informações como autor, data e mensagem do commit.


```sh
git log
```


### git branch
O comando git branch é usado para listar, criar ou deletar branch.


- Listar branch:
```sh
git branch
```
- Criar branch
```sh
git branch nome_da_branch
```


- Deletar branch
```sh
git branch -d nome_da_branch
```


- Renomer branch
```sh
git branch -m nome_antigo nome_novo
```
### git checkout
O comando git checkout é usado para trocar de branch, ou  criar uma nova branch e mudar para ela imediatamente.


- Trocar de branch
```sh
git checkout nome_do_branch
```
- Criar e mudar de branch
```sh
git checkout -b nome-nova-branch
```


### git merge
O comando git merge é usado para integrar as mudanças de um branch para outra. Por exemplo, para mesclar as mudanças de uma branch para main, você faria:


```sh
git checkout main
git merge nome-branch
```

