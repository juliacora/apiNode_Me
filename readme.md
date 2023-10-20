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
Criar pastas dentro da pasta src
```
mkdir src/routes
```
Criar arquivo dentro da pasta routes
```
touch src/routes/rotas.js
```
Abrir o VSCode
```
code .
```
Abrir o arquivo rotas.js e digitar os códigos
```
// Importar o modulo de Router do express
const { Router } = require('express');

// Instanciar o Router na variável router
const router = Router();

router.get('/listar', (request, response) => {
    response.send('Método GET: listar informações');
});
router.post('/cadastrar', (request, response) => {
    response.send('Método POST: salvar informações');
});
router.put('/user/:id', (request, response) => {
    response.send('Método PUT: atualizar informações');
});
router.delete('/user/:id', (request, response) => {
    response.send('Método DELETE: remover informações');
});

module.exports = router;

```
Abrir o arquivo app.js e adicionar o código
```
const router = require('./routes/rotas');
```
```
app.use('/api', router);
```
Atualizar projeto no gitHub
```
git add .
```
Salvar projeto e escrever comentário sobre o processo realizado
```
git commit -m 'rotas do projeto'
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