# Projeto1_EC48B_C81_ProgramacaoWebBackEnd
Projeto 1 da disciplina de Programação Web Back-End (EC48B-C81)

Biblioteca Node.js para gerenciamento de e-commerce (inspirado no AliExpress) utilizando **MongoDB** como banco de dados, com validação de campos obrigatórios e sistema de logs.

## Pré-requisitos

- Node.js (v14 ou superior)
- MongoDB (v4.4 ou superior) - local ou Atlas

## Instalação

1. Clone o repositório
2. Instale as dependências:
```bash
npm install
```
## Configure o arquivo .env com suas credenciais do MongoDB:
```bash
MONGO_URI=mongodb://localhost:27017
MONGO_DB_NAME=ecommerce_db
```
## Para MongoDB Atlas (nuvem):
```bash
MONGO_URI=mongodb+srv://usuario:senha@cluster.mongodb.net/
MONGO_DB_NAME=ecommerce_db
```
## Executar testes
```bash
node test.js
```
## Estrutura do Projeto
```bash
projeto-ecommerce-mongodb/
├── src/
│   ├── db/
│   │   └── connection.js      # Conexão com MongoDB
│   ├── models/
│   │   ├── Cliente.js         # CRUD de clientes
│   │   ├── Produto.js         # CRUD de produtos
│   │   └── Pedido.js          # Gerenciamento de pedidos
│   └── utils/
│       └── logger.js          # Sistema de logs
├── logs/
│   ├── error.log              # Logs de erros
│   └── info.log               # Logs de informações
├── test.js                    # Arquivo de testes
├── .env                       # Configurações
└── package.json
```
