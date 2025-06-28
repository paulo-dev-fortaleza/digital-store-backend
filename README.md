🛒 DIGITAL STORE BACKEND
   ----------------------
Este é o backend da aplicação **Digital Store**, uma API RESTful desenvolvida com **Node.js**, **Express** e **Sequelize**, utilizando **MySQL** como banco de dados.
O projeto oferece autenticação com JWT, testes automatizados com Jest e documentação via Swagger.

🚀 TECNOLOGIAS UTILIZADAS
    ----------------------
- **Node.js** – Ambiente de execução JavaScript
- **Express** – Framework web para APIs
- **Sequelize** – ORM para MySQL
- **JWT** – Autenticação baseada em tokens
- **Jest** + **Supertest** – Testes automatizados
- **Swagger** – Documentação da API
- **Dotenv** – Variáveis de ambiente

⚙️ INSTALAÇÃO E CONFIGURAÇÃO:
    -------------------------
✅ PRÉ -REQUISITOS

Antes de começar, você precisa ter instalado:
- Node.js (versão 16 ou superior)
- MySQL (ou MariaDB)
- Git (para clonar o repositório)
- Postman (opcional, para testar a API)

📥 CLONE O REPOSITÓRIO:
    -------------------
git clone https://github.com/paulo-dev-fortaleza/digital-store-backend.git
cd digital-store-backend

📦 INSTALE AS DEPENDENCIAS:
   ------------------------
npm install

🛠️ CONFIGURE AS VARIÁVEIS DE AMBIENTE:
    ----------------------------------
Crie um arquivo .env com base no exemplo:
cp .env.example .env

EDITE O .env COM SUAS CONFIGURAÇÕES LOCAIS, COMO:
-------------------------------------------------
DB_HOST=localhost
DB_USER=seu_usuario_mysql
DB_PASSWORD=sua_senha_mysql
DB_NAME=digital_store
JWT_SECRET=sua_chave_secreta
PORT=3000

🗃️ CONFIGURE O BANCO DE DADOS:
   ---------------------------
Certifique-se de que o MySQL está rodando e execute os comandos abaixo para criar o banco, as tabelas e popular com dados iniciais:
npx sequelize db:create
npx sequelize db:migrate
npx sequelize db:seed:all

▶️ INICIE O SSERVIDOR:
    ------------------
Em modo de desenvolvimento (com reinício automático):
npm run dev

EM MODO DE PRODUÇÃO:
--------------------
npm start

A API ESTARÁ DISPONIVÉL EM:
--------------------------
📍 http://localhost:3000
A documentação Swagger estará em:
📚 http://localhost:3000/api-docs

🧪 EXECUTE OS TESTES:
   ------------------
Para rodar os testes automatizados:
npm test

BANCO DE DADOS:
---------------
npx sequelize db:create
npx sequelize db:migrate
npx sequelize db:seed:all
