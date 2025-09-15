# 📋 Finanças Pessoais

Este é um projeto de uma aplicação web de controle de finanças pessoais, desenvolvida utilizando HTML, CSS e JavaScript. A aplicação permite o gerenciamento de transações financeiras e utiliza o json-server para simular um backend.

## 📝 Descrição

A aplicação tem como objetivo gerenciar transações financeiras de forma simples e eficaz. As funcionalidades incluem:

- 🆕 **Criar transações** com nome e valor.
- 🔁 **Editar transações** já cadastradas.
- 🗑️ **Excluir transações**.
- 💸 **Visualizar o saldo total**, que é calculado a partir das transações.
- 🖥️ **Interface interativa**, onde todas as mudanças (criação, edição e exclusão de transações) acontecem sem atualizar a página.

A aplicação utiliza o json-server como backend para simular uma API REST que armazena as transações em um arquivo `db.json`.

## ⚙️ Funcionalidades

  - **Adicionar nova transação** através de um formulário.
  - **Visualizar todas as transações** salvas no backend.
  - **Editar transações** enviando uma requisição PUT.
  - **Excluir transações** com uma requisição DELETE.
  - **Cálculo do saldo total** automaticamente ao criar, editar ou excluir transações.

## 🛠️ Tecnologias Usadas

- ![HTML](https://img.shields.io/badge/HTML-E34F26?style=for-the-badge&logo=html5&logoColor=white) **HTML** – Estruturação da página.
- ![CSS](https://img.shields.io/badge/CSS-1572B6?style=for-the-badge&logo=css3&logoColor=white) **CSS** – Estilização da página.
- ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black) **JavaScript** – Lógica de funcionamento da aplicação.
- ![json-server](https://img.shields.io/badge/json--server-000000?style=for-the-badge&logo=json&logoColor=white) **json-server** – Simulação de uma API REST.

## 🗂️ Estrutura de Pastas e Arquivos

Aqui está uma visão geral da estrutura do projeto com explicações dos arquivos importantes:

```

easy-finances/
├─ node\_modules/          # Dependências do projeto (gerado automaticamente)
├─ db.json                # Banco de dados "fake" para o json-server
├─ index.html             # Página principal da aplicação
├─ index.js               # Lógica JavaScript para a aplicação
├─ package.json           # Define as dependências e scripts do projeto
├─ package-lock.json      # Grava a versão exata das dependências instaladas
├─ README.md              # Documentação do projeto (este arquivo)
└─ style.css              # Estilos CSS para a aplicação

````

## 🚀 Como Rodar o Projeto Localmente

**Pré-requisitos:** Node.js (recomendado versão 18+).

### 1) Clonar o repositório

```bash
git clone https://github.com/RaphaelOkuyama/easy-finances.git
cd easy-finances
````

### 2) Instalar as dependências

```bash
npm install
```

### 3) Subir a API (json-server)

```bash
npm run serve
```

> A API estará disponível em: `http://localhost:3000`

### 4) Rodar o app

Abra o arquivo `index.html` no **Live Server** ou diretamente no navegador.

## 🛣️ Endpoint `/transactions`

A API simula um backend com o endpoint `/transactions`, que permite as seguintes operações:

* **`POST /transactions`** – Cria uma nova transação financeira com `nome` e `valor`.
* **`GET /transactions`** – Recupera todas as transações armazenadas no backend.
* **`PUT /transactions/:id`** – Atualiza os dados de uma transação específica (por exemplo, `nome` ou `valor`) através do `id`.
* **`DELETE /transactions/:id`** – Exclui uma transação específica usando o `id` da transação.

Esses endpoints são gerenciados pelo json-server, permitindo a manipulação das transações sem necessidade de um backend real.

## 📦 Scripts Disponíveis

* `npm run serve` – Inicia o json-server (simulando a API).

## 🤝 Contribuições

Sugestões, melhorias e contribuições são bem-vindas! Abra uma issue ou envie um pull request.

## 📄 Licença

Este projeto está licenciado sob a **MIT License**.
Consulte o arquivo [LICENSE](./LICENSE) para o texto completo.

Copyright (c) 2025 Raphael Okuyama
