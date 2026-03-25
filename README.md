# Criar Repositório

logar no github
criar um novo repositório
- digitar nome
- ativar o README
- e selecionar o gitignore como: NODE

# Baixar o repositório

organizar a pasta
abrir o git bash here 
- rodar o comando: git clone URL DO REPOSITÓRIO
OBS: Ctrl+c Ctrl+v não funciona! 

# mudar a política de scripts externos

abrir o power shell como admin:
- digitar o comando: 
Set-ExecutionPolicy RemoteSigned
e 's' para sim!


# para criação da api (NODE DEVE ESTAR INSTALADO NA MÁQUINA):
ABRIR A PASTA DO PROJETO NO VS CODE 

ABRIR O TERMINAL DO VSCODE E DIGITAR:

node -v

npm init -y

npm install express

# criar arquivo index.js:


const express = require("express");
const app = express();


app.get("/", (req, res) => {
  res.send("Hello World!");
});


app.listen(3005, () => {
  console.log("Servidor on");
});



# PARA RODAR 
NO TERMINAL: 

node index.js

E NO NAVEGADOR:

http://localhost:3005/

# Para fazer o commit 

Abrir o git bash here dentro da pasta git e rodas os seguintes comandos:

git status
git add .
git status
git commit -m "NOME DO COMMIT"
git push

OBS: se for a primeira vez usando o git na máquina:

git config --global user.name "Your Name"
git config --global user.email "Your EMail "

E ACEITAR NA CAIXINHA QUE ABRE!

# Rodar o projeto apenas:

Clonar o projeto!
no terminal: npm i 

e seguir as demais etapas já descritas

# Branch

1)Criar uma Branch
EX: 'dev' 

2)No terminal: 
- git fetch
- git checkout 'dev'

# pull request

1) Clicar no botão 'Compare & pull request' que aparece no github
2) Clicar em new pull request
3) Clicar em 'Create pull request' OBS: se quiser colocar um comentário, pode colocar no campo de texto
4) Clicar em 'Merge pull request' para juntar a branch 'dev' com a 'main'
5) Clicar em 'Confirm merge'