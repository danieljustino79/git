# Git
Sistema distribuído de controle de versão com repositório sobre um diretório do sistema operacional (Windows, Linux ou Mac).

## Lifecycle
untracked, unmodified, modified, staged

## Versão
git --version

## Configuração
git config --global user.name "nome"  
git config --global user.email "e@mail"  

git config user.name  
git config --list

## Comandos básicos
git status  
git add .  (lifecycle: staged)  
git commit -m "msg"  
git log

### git log
git log --author="sam"  
git shortlog  
git log --graph  

## Outros comandos
git show  
git diff  
git checkout  (undo na alteração em lifecycle: modified)  
git reset HEAD  (undo na alteração em lifecycle: staged)  


### git show
git show 71bc6dc7 (8 digitos)  

### git diff
git diff --name-only

### git reset
git reset HEAD nomeArquivo  
git reset --soft commitDestino  
git reset --soft  (undo no commit e lifecycle: staged)  
git reset --mixed  (undo no commit e lifecycle: modified)  
git reset --hard  (undo no commit e lifecycle: unmodified)  

## Generate ssh key 
[help.github.com](https://help.github.com/en/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)  
ssh-keygen "email@prov.com"  
cat id_rsa.pub  

## Quick setup
### New repository on the command line
git init  
git add README.md  
git commit -m "first commit"  
git remote add origin git@github.com:userOwner/git.git  
git push -u origin master  

### Push an existing repository from the command line
git remote add origin  git@github.com:userOwner/git.git  
git push -u origin master  

## Git remote
git remote

### git remote
git remote -v

https://www.udemy.com/git-e-github-para-iniciantes/learn/lecture/5120550#overview