# Back End do projeto MyEdu para o Bootcamp Tera 

<p align="center">
<img src="https://img.shields.io/static/v1?label=STATUS&message=FINALIZADO&color=GREEN&style=for-the-badge"/>
</p>

## Executar o projeto

Projeto Clonar git clone `https://github.com/BrunoFelixB/myedu-backend.git`

Configure e ative seu ambiente virtual

Requisitos de instalação `npm install`

Dependências: `axios, cors, dontenv-safe, express, mongoose, node-fetch, nodemon, schema`


### Primeiro - rodar o comando para iniciar o servidor:

```
npm run dev

```
O comando irá ligar o servidor e o mesmo funcionará através da porta 3000.


### Método GET

```
http://localhost:3000/users/all

```
está rota irá retornar todas as universidades armazenadas no banco de dados.


### Método para buscar a universidade por id:

### Método GET

o id deve ser passado por parâmetro

```
http://localhost:3000/users/:id

```
essa rota irá retorna a universidade referente ao ID.

### Método para Login de usuário:

### Método POST

```
http://localhost:3000/users/create


devem ser passados pelo body os seguintes comandos: 
{
	"email": "string",
	"password": "string"
}


```

```

A api responderá com um Token importante para autenticação.

```




### Método para cadastro de usuário:

### Método POST

```
http://localhost:3000/users/create


devem ser passados pelo body os seguintes comandos: 

{
  "name":"string",
  "email":"string",
  "password":"string",
  "course":"string"
}


```


### Método para atualizar usuário:

### Método PATCH

o id deve ser passado por parâmetro

```
http://localhost:3000/users/update/id


devem ser passados pelo body os seguintes comandos: 

{
  "course":"string"
}

```

Essa rota irá atualizar o curso do usuário.

### Método para deletar usuário:

### Método DELETE

o id deve ser passado por parâmetro

```
http://localhost:3000/users/delete/id

```

Essa rota irá deletar o usuário do banco de dados.

