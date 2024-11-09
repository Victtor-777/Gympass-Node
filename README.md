# GymPass (Back-end API)

API Back-end para uma aplicação para check-ins em academias, estilo gympass, aplicando conceitos do SOLID, Design Patterns, Docker para iniciar o banco de dados, JWT e Refresh Token, RBAC e diversos outros conceitos. A aplicação está bem completa com todas as funcinalidades de um gympass e com validações de dados utilizando o ZOD, testes unitários e e2e, além de utilizar o github actions para um CI/CD.

## RFs (Requisitos funcionais)

- [x] Deve ser possível se cadastrar;
- [x] Deve ser possível se autenticar;
- [x] Deve ser possível obter o perfil de um usuário logado;
- [x] Deve ser possível obter o número de check-ins realizados pelo usuário logado;
- [x] Deve ser possível o usuário obter seu histórico de check-ins;
- [x] Deve ser possível o usuário buscar academias próximas (até 10km);
- [x] Deve ser possível o usuário buscar academais pelo nome;
- [x] Deve ser possível o usuário realizar check-in em uma academia;
- [x] Deve ser possível validar o check-in de um usuário;
- [x] Deve ser possível cadastrar uma academia;

## RNs (Regras de negócio)

- [x] O usuário não deve poder se cadastrar com um e-mail duplicado;
- [x] O usuário não pode fazer 2 check-ins no mesmo dia;
- [x] O usuário não pode fazer check-in se não estiver perto (100m) da academia;
- [x] O check-in só pode ser validado até 20 minutos após ser criado;
- [x] O check-in só pode ser validado por administradores;
- [x] A academia só pode ser cadastrada por administradores;

## RNFs (Requisitos não funcionais)

- [x] A senha do usuário precisa estar criptografada;
- [x] Os dados da aplicação precisam estar persistidos em um banco PostgreeSQL;
- [x] Todas listas de dados precisam estar paginadas com 20 itens por página;
- [x] O usuário deve ser indentificado por um JWT (JSON Web Token);

## ⚙ Clonando Projeto

```
# Faça o clone do repotório
  git clone git@github.com/Victtor-777/Gympass-Node.git

# Instalar as dependências do projeto
  npm install

# Rodar as migrations do projeto para criar o banco de dados
  npx prisma migrate dev

# Executando o projeto no ambiente de desenvolvimento
  npm run dev
```

## 🚀 Tecnologias

- Node.js
- TypeScript
- Fastify
- Prisma
- Docker
- Zod
- Vitest
- MySQL
