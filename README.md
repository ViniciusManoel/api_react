# Projeto de treinamento para o consumo de dados de uma API utilizando o React e o Axios

## 1º Passo: Abrir o [Repl.it](http://replit.com)

### Para desenvolver uma API de exemplo:
1º - Crie um cadastro, caso não o tenha;\
2º - Crie um novo repositorio, clicando em `+` localizado no canto superior direito;\
3º - Escolha como linguagem o `NodeJS` e dê um nome ao vosso repositório.

## 2º Passo: A API 

```node

var cars = '[' +
  '{"id":1,"marca":"Honda","modelo":"HRV"},'+
  '{"id":2,"marca":"Volkswagen","modelo":"Golf"},'+
  '{"id":3,"marca":"Fiat","modelo":"Toro"},'+
  '{"id":4,"marca":"GM","modelo":"Tracker"},'+
  '{"id":5,"marca":"Ford","modelo":"Ranger"}'+
  ']';
var http = require('http');
var server = http.createServer(function(request,response){
  response.setHeader('Access-Control-Allow-Origin','*')
  response.writeHeader(200,{"Content-Type":"text/html"})
  response.write(cars)
  response.end()
});
server.listen(3000)

```
## 3º Passo: Rodar o servidor no Repl.it 
Verifique possíveis erros e o mantenha rodando para que o sistema possa consumir a vossa API de teste.

## 4º Passo: Como executar?
Precisaremos do `Node` instalado no vosso computador, assim como o `React` e o `Axios`

### instalação do react e axios:
npm init
npx create-react-app proj-name
cd proj-name
npm install axios

### iniciando o react:
npm start