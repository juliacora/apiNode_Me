# Documentação
Copiar a url do projeto

Apagar pasta no PC

Para o repositório na sua máquina
```
git clone URL_REPOSITORIO
```
Acessar pasta
```
cd NOME_REPOSITORIO
```
Reinstalar os pacotes da aplicação
```
npm i
```
Criar arquivo .env na raiz do projeto

* Ctrl + o: Salvar o arquivo

* Enter: Confirmar

* Ctrl + x: Fechar o arquivo
```
nano .env
```
Digitar no arquivo .env
```
PORT = 3008
```
Adicionar arquivo .env no .gitignor
```
nano .gitignore
```
```
.env
```
Abrir o VSCode
```
code .
```
Criar arquivo de exemplo para para as variáveis necessárias da aplicação
```
nano .env.example
```
Adicionar no arquivo .env.example
```
PORT =
```
Abrir o arquivo app.js e digitar o código
```
const express = require('express');
```
```
const dotenv = require('dotenv').config();
```
```
const app = express();
```
```
app.set('port', process.env.PORT || 3333);
```
```
module.exports = app;
```
Abrir o arquivo server.js e digitar os códigos
```
const app = require('./app');
```
```
const port = app.get('port');
```
```
app.listen(port, () => {
    console.log(`Running on port ${ port }!`);
});
```
Abrir o arquivo package.json e alterar a chave 'scripts'
```
"start":"nodemon src/server.js"
```
Rodar o comando no termial com gitBash
```
npm run start
```
Atualizar projeto no gitHub
```
git add .
```
Salvar projeto e escrever comentário sobre o processo realizado
```
git commit -m 'configuração do projeto'
```
Enviar os arquivos atualizados para o gitHub
```
git push
```
Atualize a página no gitHub e verifique se os arquivos foram atualizados

* Com o projeto no servidor remoto podemos remover os arquivos na nossa máquina
```
cd ..
```
Fechar o VSCode com o projeto aberto
```
rm -rf projetoBackend