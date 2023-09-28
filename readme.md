# Documentação
Criar pasta para a aplicação
```
mkdir projetoBackend
```
Acessar pasta
```
cd projetoBackend
```
Criar arquivo para documentar projeto
```
touch readme.md
```
Iniciar o gerenciador de pacotes Node
```
npm init -y
```
Instalar os pacotes
```
npm i express nodemon dotenv
```
Abrir o VSCode
```
code .
```
Criar arquivo .gitignore
```
nano .gitignore
```
Adicionar no arquivo .gitignore o nome da pasta criada após a instalação dos pacotes
```
node_modules
```
Criar estrutura de arquivos e pastas
```
mkdir src
```
Criar arquivos dentro da pasta src
```
touch src/app.js
```
```
touch src/server.js
```
Criar pastas dentro da pasta src
```
mkdir src/config
```
```
mkdir src/controllers
```
```
mkdir src/routes
```
Enviar estrutura do projeto para o gitHub
```
git init
```
Informar o seu nome e email
```
git config --global user.name "FIRST_NAME"
```
```
 git config --global user.email "EMAIL@EXAMPLE.COM"
```
Verificar arquivos que serão enviados ao gitHub
```
git status
```
Adicionar todos arquivos ao versionamento
```
git add .
```
Salvar projeto e escrever comentário sobre o processo realizado
```
git commit -m 'estrutura do projeto'
```
De volta ao terminal, executar o comando para definir a branch main
```
git branch -M main
```
Colar a URL do seu repositório copiada
```
git remote add origin COLAR_URL
```
Enviar os arquivos para o gitHub
```
git push -u origin main
```
Com o projeto no servidor remoto podemos remover os arquivos na nossa máquina
```
cd ..
```
Fechar o VSCode com o projeto aberto
```
rm -rf projetoBackend
