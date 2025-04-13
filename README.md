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

### 🐍 2. Crie e Ative um Ambiente Virtual dentro da pasta do repositório criado:

```bash
python -m venv venv
.\venv\Scripts\activate   # Windows
```

### 📦 3. Instale as Dependências

```bash
pip install -r requeriments.txt
```

## ▶️ 4. Rode o Servidor

```bash
uvicorn app.main:app --reload
```

Após isso, o servidor estará disponível em: http://localhost:8000

## ⚙️ Rodando o Backend via Docker

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

⚠️ usuários de windows, importante, [Verifique se a virtualização da sua máquina está ativada na BIOS](https://support.microsoft.com/pt-br/windows/habilitar-a-virtualiza%C3%A7%C3%A3o-no-windows-c5578302-6e43-4b4b-a449-8ced115f58e1), pois ela é fundamental para habilitação do WSL2. Em seguida, você deve seguir os passos de instalação e habilitação do [WSL2](https://learn.microsoft.com/pt-br/windows/wsl/install), para execução do Docker.

## 🧱 🚀 3. Construa a Imagem e Rode o container

Na pasta do projeto, deverá conter também o repositório front-end (git clone https://github.com/victorazevedo0/MVP_Sprint-3_Front-end.git) conforme descrito no README.md do front-end, pois lá terá o arquivo docker-compose.yml.
Ao entrar na pasta do front-end, rodar o comando abaixo (com isso seu projeto estará back-end e front-end rodando via docker):

```bash
docker-compose up --build
```

### Segue estrutura do projeto para rodar via docker:
```
[pasta_que_você_criou]/
    ├── MVP_Sprint-3_back-end/ 
____├── MVP_Sprint-3_Front-end 
_____________├── docker-compose.yml
```

A API estará disponível em: http://localhost:8000
📌 Endpoints da API

Abaixo estão listados alguns dos principais endpoints disponíveis:
Método | Rota | Descrição
------ |------| ---------
GET | /api/v1/orders | Lista todos os pedidos
GET | /api/v1/orders/{id} | Retorna um pedido específico
POST | /api/v1/orders | Cria um novo pedido
PUT | /api/v1/orders/{id} | Atualiza um pedido existente
DELETE | /api/v1/orders/{id} | Remove um pedido

    Acesse a documentação interativa em: http://localhost:8000/docs
**Desenvolvido por Victor Azevedo 💻**
