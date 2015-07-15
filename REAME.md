## Modelo de Projeto Express

Pequeno guia descrevendo uma maneira de organizar e preparar um novo projeto com Express. Abordando desde a estrutura como algumas tecnologias úteis para o desenrolar do desenvolvimento.

### Estrutura de pastas e arquivos

Abaixo segue a estrutura de pastas e arquivos de forma simplicada de como poderia ser iniciado um projeto com express. 

```javacript
project/
  app/
    controllers/
    models/
    middlewares/
  config/
    routes.js
  migrations/
  public/
    images/
    js/
    css/
    vendor/
    views/
  tests/
  database.json
  package.json
  server.js

```

### Módulos essências 

#### [Morgan](https://github.com/expressjs/morgan)

HTTP request logger middleware for node.js

#### [Body Parser](https://github.com/expressjs/body-parser)

Node.js body parsing middleware.

#### [Method Override](https://github.com/expressjs/method-override)

Lets you use HTTP verbs such as PUT or DELETE in places where the client doesn't support it.


### Módulos para persistência de dados 

#### [PG](https://github.com/voxpelli/node-connect-pg-simple)

A simple, minimal PostgreSQL session store for Express/Connect.

#### [DB Migrate](https://github.com/db-migrate/node-db-migrate)

Database migration framework for node.js.

### Módulos para testes

#### [Jest](https://facebook.github.io/jest/)

Painless JavaScript Unit Testing.

### Angular

Seguindo essa estrutura não possuímos views, no lugar temos o diretório  public que irá conter todo o frontend.  E nele será utilizado o angular.js. Assim é possível criar um singlepage application  que irá consumir uma api criada com o backend em javascript  com express e node.js.  

#### Bower

configuração para o bower. Crie o arquivo .bowerrc na pasta public com o seguinte template. Isso fára que nossos módulos do Bower sejam instaladas em uma pasta chamada vendor em public. 

```
{
  "directory": "vendor"
}
```

