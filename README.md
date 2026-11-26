# Git Flow

## Configuração inicial

```bash
git config --global user.name "Seu Nome"
git config --global user.email "cheirapeido@gmail.com"
git config --list
```

## Criar e clonar repositórios

```bash
git init
git clone URL_DO_REPOSITORIO
```

## Verificar alterações

```bash
git status
git diff
git log
git log --oneline
```

## Criar commits

```bash
git add .
git add nome-do-arquivo
git commit -m "mensagem do commit"
```

## Enviar alterações para o GitHub

```bash
git push
git push origin main
git pull
git fetch
```

## Trabalhar com branches

```bash
git branch
git branch nome-da-branch
git switch nome-da-branch
git switch -c nova-branch
git checkout nome-da-branch
git push -u origin nome-da-branch
```

## juntar branches

```bash
git merge nome-da-branch
git merge --abort
```

## Corrigir commits

```bash
git commit --amend -m "nova mensagem"
git reset --soft HEAD~1
git reset --mixed HEAD~1
git revert HEAD
```

## Desfazer alterações

```bash
git restore nome-do-arquivo
git restore --staged nome-do-arquivo
git reset --hard HEAD
```

## Git Flow

Principais branches:

- main: versão estável do projeto.
- develop: desenvolvimento do projeto.
- feature: criação de novas funcionalidades.
- release: preparação de uma versão.
- hotfix: correção de problemas urgentes.

Exemplo de criação de branch:

```bash
git switch -c develop
git switch -c feature/cadastro
```