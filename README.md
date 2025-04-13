# 🛒 Loja Virtual - Backend

Este é o **backend** do projeto **Loja Virtual**, uma aplicação web desenvolvida como parte do MVP acadêmico da Sprint 3.

A API foi construída com **FastAPI**, utilizando **SQLite** para persistência de dados, adotando a arquitetura **MVC** e comunicação via **REST API** com o frontend. Ela é responsável por gerenciar os **pedidos** e **produtos** do sistema.

---

## 🚀 Tecnologias Utilizadas

- 🐍 Python 3.12+
- ⚡ FastAPI
- 🛠️ SQLAlchemy
- 💾 SQLite
- 🔥 Uvicorn
- 🐳 Docker

---

## ⚙️ Rodando o Backend Localmente

Siga os passos abaixo para executar o projeto no seu ambiente local.

### 📥 1. Clone o Repositório

Crie uma pasta e clone o projeto abaixo:

```bash
git clone https://github.com/victorazevedo0/MVP_Sprint-3_back-end.git
```

## 🐍 2. Crie e Ative um Ambiente Virtual

```bash
python -m venv venv
.\venv\Scripts\activate   # Windows
```

## 📦 3. Instale as Dependências

```bash
pip install -r requeriments.txt
```

## ▶️ 4. Rode o Servidor

```bash
uvicorn app.main:app --reload
```

Após isso, o servidor estará disponível em: http://localhost:8000

## ⚙️ Rodando o Backend no Docker

Siga os passos abaixo para executar o projeto no seu ambiente local.

### 📥 1. Clone o Repositório

Crie uma pasta de clone o projeto abaixo:
```bash
git clone https://github.com/victorazevedo0/MVP_Sprint-3_back-end.git
```

## 🐳 2. Rodando com Docker

📌 Pré-requisitos

Instale o Docker de acordo com seu sistema operacional:

    📥 Windows
    📥 Ubuntu
    📥 MacOS

    ⚠️ Usuários Windows: certifique-se de que a virtualização está habilitada na BIOS e que o WSL2 está corretamente instalado e configurado.

## 🧱 🚀 3. Construa a Imagem e Rode o container

```bash
docker-compose up --build
```
A API estará disponível em: http://localhost:8000
📌 Endpoints da API

Abaixo estão listados alguns dos principais endpoints disponíveis:
Método	Rota	Descrição
GET	/api/v1/orders	Lista todos os pedidos
GET	/api/v1/orders/{id}	Retorna um pedido específico
POST /api/v1/orders	Cria um novo pedido
PUT	/api/v1/orders/{id}	Atualiza um pedido existente
DELETE	/api/v1/orders/{id}	Remove um pedido

    Acesse a documentação interativa em: http://localhost:8000/docs
**Desenvolvido por Victor Azevedo 💻**
