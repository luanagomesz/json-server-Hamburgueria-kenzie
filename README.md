# json-server-base

Esse é o repositório com a base de JSON-Server + JSON-Server-Auth já configurada, feita para ser usada no desenvolvimento das API's nos Capstones do Q2.

## Endpoints



### Cadastro

POST /register <br/>
POST /signup <br/>
POST /users

Qualquer um desses 3 endpoints irá cadastrar o usuário na lista de "Users", sendo que os campos obrigatórios são os de email e password.
Você pode ficar a vontade para adicionar qualquer outra propriedade no corpo do cadastro dos usuários.


### Login

POST /login <br/>
POST /signin

Qualquer um desses 2 endpoints pode ser usado para realizar login com um dos usuários cadastrados na lista de "Users"

### Posts

POST /posts

para criar um post o usuario deve estar logado, é passado o userID na requisição, junto do campo titulo e texto, o post é atrelado ao user

também é possivel dar um get para ver todos posts, não é necessario estar logado

GET /posts/

também é possivel pegar posts de um usuario especifico usando userId

GET /posts/?userId={value}


### Newsletter

GET /newsletter

pode ser vizualizado por qualquer usuario logado e com token.
