# API - Node.js (JavaScript) + Express + Prisma + MongoDB

Este projeto é uma API REST simples feita em **JavaScript (Node.js)** usando **Express** e **Prisma** conectada a um banco **MongoDB** (ex.: Atlas).

---

## 🧰 Tecnologias usadas

- **Node.js** (projeto em ESM — usa `import/export`)
- **Express** (rotas HTTP)
- **Prisma** (ORM / Client)
- **MongoDB** (Atlas ou local)

---

## ✅ Pré-requisitos

Antes de rodar, você precisa ter:

1. **Node.js** instalado (recomendado 18+)
2. **NPM** (já vem com o Node)
3. Uma string de conexão do **MongoDB** (ex.: MongoDB Atlas)

Para conferir se está tudo ok:

```bash
node -v
npm -v
```

## 🚀 Como rodar o projeto

### 1. Instalar as dependências

Execute o comando abaixo para instalar todas as dependências do projeto:

```bash
npm install
```

### 2. Validar o schema do Prisma

Verifica se o arquivo `schema.prisma` está correto:

```bash
npx prisma validate
```

### 3. Gerar o Prisma Client (obrigatório)

Gera o client do Prisma, necessário para a aplicação funcionar:

```bash
npx prisma generate
```

### 4. Sincronizar o schema com o MongoDB

Aplica o schema no banco de dados MongoDB:

```bash
npx prisma db push
```

### 5. Subir o servidor

Inicia o servidor da aplicação:

```bash
node --watch server.js
```

Após executar esse comando, a API estará disponível em:

```
http://localhost:3000
```
