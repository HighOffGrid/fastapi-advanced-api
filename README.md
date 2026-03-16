# FastAPI Docker PostgreSQL API

API backend desenvolvida com FastAPI, utilizando PostgreSQL como banco de dados e Docker para containerização da aplicação.

Projeto criado para estudo de deploy e execução de APIs utilizando containers.

---

Tecnologias:
	•	FastAPI
	•	PostgreSQL
	•	Docker
	•	SQLAlchemy
	•	Pydantic
	•	Uvicorn

---

Funcionalidades:
	•	API REST com FastAPI
	•	Integração com PostgreSQL
	•	Containerização com Docker
	•	Estrutura básica para aplicações backend

---

## Arquitetura


Client
   │
   ▼
FastAPI API
   │
   ▼
SQLAlchemy ORM
   │
   ▼
PostgreSQL Database

---

## Objetivo


Este projeto foi desenvolvido para prática de desenvolvimento backend com FastAPI e uso de containers com Docker.

---

## Rodando o projeto


Clone o repositório:

```bash
git clone https://github.com/seuuser/fastapi-docker-postgresql
cd FastAPI avançado

---

Instale as dependências:

pip install -r requirements.txt

---

## Executando a API

uvicorn app.main:app --reload

Swagger UI: http://127.0.0.1:8000/docs

ReDoc: http://127.0.0.1:8000/redoc
