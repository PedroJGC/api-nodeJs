# API RESTful Node.js

Este projeto foi desenvolvido durante o curso Fullstack da Rocketseat e consiste em uma API RESTful construída com Node.js puro, sem frameworks externos.

## Sobre o Projeto

Esta API implementa um CRUD básico para produtos utilizando apenas módulos nativos do Node.js (`node:http`, `node:fs`), demonstrando conceitos fundamentais de desenvolvimento backend como:

- Criação de servidor HTTP
- Persistência de dados em arquivo JSON
- Roteamento de requisições
- Middlewares
- Tratamento de parâmetros de URL e query string

## Estrutura do Projeto

```
src/
├── database.js        # Classe para persistência de dados em JSON
├── db.json            # Arquivo de banco de dados
├── routes.js          # Definição das rotas da aplicação
├── server.js          # Configuração do servidor HTTP
├── middlewares/
│   ├── jsonBodyHandler.js  # Middleware para processar corpo JSON
│   └── routeHandler.js     # Middleware para roteamento
└── utils/
    ├── extract-query-params.js  # Extração de parâmetros de consulta
    └── parseRoutePath.js        # Conversão de path para regex
```

## Funcionalidades

- **GET /products**: Lista todos os produtos
- **POST /products**: Cria um novo produto
- **DELETE /products/:id**: Remove um produto pelo ID

## Como Executar

1. Clone este repositório
2. Navegue até a pasta do projeto
3. Execute o servidor:

```bash
node src/server.js
```

O servidor estará disponível em `http://localhost:3333`.

## Tecnologias Utilizadas

- Node.js puro (sem frameworks externos)
- JavaScript com ECMAScript Modules
- Persistência em arquivo JSON
- HTTP nativo do Node.js

## Aprendizados

Este projeto demonstra como construir uma API RESTful do zero, sem depender de frameworks como Express, entendendo os conceitos fundamentais de:

- Streams no Node.js
- Middlewares e pipeline de requisições
- Roteamento com expressões regulares
- Manipulação de arquivos
- Padrões de projeto para APIs
