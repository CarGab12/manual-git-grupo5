## 1. Introdução
O Git é um sistema de controle de versões amplamente utilizado por desenvolvedores. O GitHub é uma plataforma online que hospeda repositórios Git e permite colaboração em projetos.

Este manual apresenta os principais comandos para usar o Git e publicar projetos no GitHub, com um passo a passo prático.

## 2. Instalação
Baixe e instale o Git:

Site oficial: https://git-scm.com

Após instalar, abra o terminal (Git Bash no Windows ou Terminal no macOS/Linux).

## 3. Configuração Inicial
Antes de começar a usar o Git, configure seu nome e e-mail:

git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"

Verifique a configuração:
git config --list

## 4. Iniciando um Projeto
Criar um repositório local: git init
Isso cria um repositório Git vazio na pasta atual.

Clonar um repositório do GitHub: git clone https://github.com/usuario/nome-do-repositorio.git

## 5. Ciclo Básico de Trabalho
Verificar o status dos arquivos: git status
Adicionar arquivos ao staging: git add nome_arquivo.extensao
Ou todos os arquivos modificados: git add .
Criar um commit: git commit -m "Mensagem explicando a alteração"

## 6. Conectar e Enviar para o GitHub
Adicionar repositório remoto (apenas uma vez): git remote add origin https://github.com/usuario/nome-do-repositorio.git
Enviar o código (push): git push -u origin main
Atualizar com alterações do GitHub (pull): git pull origin main

## 7. Trabalhar com Branches
Criar nova branch: git branch nome-da-branch
Trocar de branch: git checkout nome-da-branch
Criar e trocar ao mesmo tempo: git checkout -b nome-da-branch
Mesclar uma branch: git merge nome-da-branch

## 8. Corrigir ou Desfazer
Remover arquivo do staging: git reset nome_arquivo
Desfazer alterações no arquivo: git checkout -- nome_arquivo

## 9. Visualizar Histórico
Ver commits anteriores: git log
Ver de forma resumida: git log --oneline

## 10. Boas Práticas
Use mensagens de commit claras e objetivas.

Commit frequente evita perda de trabalho.

Use branches para novas funcionalidades.

Sempre puxe (pull) antes de começar a trabalhar.
