# Introdução ao Git e Github

### Comandos básicos

**Windows**

dir - lista os diretórios da pasta atual

cd - navegar entre as pastas

cd / - ir para a base do diretório

cd .. - retroceder 1 diretório

cls - limpar a tela

mkdir - cria uma pasta

\> - redirecionador de fluxo

del - deleta arquivos de uma pasta

rmdir - deleta uma pasta

**Linux**

ls - lista os diretórios da pasta atual

cd - navegar entre as pastas

cd / - ir para a base do diretório

cd .. - retroceder 1 diretório

clear - limpar a tela

ctrl + L - atalho para limpar

mkdir - cria uma pasta

sudo su - permissão

\> - redirecionador de fluxo

rm -rf -deleta tudo dentro da pasta

ls -a - mostra pastas ocultas

### Entendendo Git

SHA1

É um algoritmo de encriptação, uma forma curta de representar um arquivo.

O git utiliza isso para verificar o estado atual de um arquivo de uma forma rápida e fácil.

### Objetos internos do Git

**Blob:** Arquivos ficam guardados dentro do blob, que contém metadados (tipo do objeto, tamanho do arquivo, “\0” e o conteúdo desse arquivo) 

‘blob 9\0conteudo’

**Tree:** Armazenam blob e apontam para tipos de blobs diferentes. Também guardam o nome do arquivo. É responsável por montar toda a estrutura de onde está os arquivos.

**Commit:** Aponta para uma árvore, aponta para o último commit realizado, aponta para o autor e para a mensagem do commit. Possuem também um timestamp, com a data e hora de quando foi criado.

Em resumo o git é um sistema distribuído e seguro.

### Chaves SSH e Tokens

SSH: É uma forma de criar uma conexão segura entre o computador e o servidor.

### Configurando o usuário e o email global no git

git config --global user.email ""

git config --global user.name ""

### Ciclo de vida no Git

git init - inicializa um repositório

git status - monitora os status dos arquivos

git add nomeArquivo - modifica o status dos arquivo para staged

git add * - modifica todos os arquivos pendentes

git commit -m "mensagem” - cria o commit com mensagem

git remote add origin adress -adiciona repositório local ao github

git branch -M main

git push -u origin main - empurra o repositório no github

git clone enderecoHttps - clona um repositório usando o endereço

git remote -v - mostra para onde os repositórios estão apontados