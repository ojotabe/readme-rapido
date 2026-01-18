# API de Livros – Tech Challenge

![Versão do Python](https://img.shields.io/badge/python-3.12-blue)
![FastAPI](https://img.shields.io/badge/FastAPI-0.121.0-green)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-16.0-blue)
![Docker](https://img.shields.io/badge/Docker-Enabled-blue)
![Arquitetura Limpa](https://img.shields.io/badge/Architecture-Clean-orange)

Uma API RESTful robusta construída com **FastAPI** para gerenciar, consultar e analisar dados de livros. Este projeto é uma solução de um Tech Challenge que integra web scraping (ETL), migrações de banco de dados e análises estatísticas de coleções de livros em um serviço único e coeso.

---

## 📋 Sumário

- Funcionalidades
- Arquitetura
- Stack Tecnológica
- Primeiros Passos
- Uso
- Documentação da API
- Estrutura do Projeto
- Contribuindo
- Autor

---

## 🚀 Funcionalidades

### 📚 Gerenciamento de Livros
- Navegação no Catálogo (lista paginada)
- Livros mais bem avaliados
- Busca por título ou categoria
- Filtro por faixa de preço
- Visualização detalhada

### 📊 Análises e Estatísticas
- Estatísticas gerais do mercado
- Métricas por categoria

### ⚙️ Administração
- Migrações de banco de dados
- ETL automatizado
- Health checks

---

## 🏗 Arquitetura

O projeto segue o padrão **Clean Architecture**, promovendo escalabilidade e manutenibilidade.

---

## 🛠 Stack Tecnológica

- Python 3.12+
- FastAPI
- PostgreSQL 16
- SQLAlchemy
- Alembic
- Poetry
- Docker & Docker Compose

---

## 🏁 Primeiros Passos

### Pré-requisitos
- Docker e Docker Compose
- Python 3.12+ e Poetry

### Instalação
```bash
git clone https://github.com/yuriperim/FIAP-tech_challenge-books_api.git
cd FIAP-tech_challenge-books_api
```

### Configuração
```bash
cp .env.development .env
```

---

## 🎮 Uso

### Docker
```bash
docker compose up --build
```

### Local
```bash
poetry install
poetry run alembic upgrade head
poetry run uvicorn src.books_api.main:app --reload
```

---

## 📖 Documentação da API

- Swagger: http://localhost:8000/docs
- ReDoc: http://localhost:8000/redoc

---

## 📂 Estrutura do Projeto

```text
src/books_api/
├── main.py
├── alembic/
├── models/
├── routers/
└── services/
```

---

## 🤝 Contribuindo

Fork → Branch → Commit → Push → Pull Request

---

## 👤 Autor

**Yuri Perim**  
Email: yuriperim@gmail.com
