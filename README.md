
# FastAPI Docker PostgreSQL API


API backend desenvolvida com FastAPI, utilizando PostgreSQL como banco de dados e Docker para containerização da aplicação.

Projeto criado para estudo de deploy e execução de APIs utilizando containers.

Tecnologias
	•	FastAPI
	•	PostgreSQL
	•	Docker
	•	SQLAlchemy
	•	Pydantic
	•	Uvicorn

Funcionalidades
	•	API REST com FastAPI
	•	Integração com PostgreSQL
	•	Containerização com Docker
	•	Estrutura básica para aplicações backend


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


## Estrutura do Projeto


project/
│
├── app/
│   ├── models/        # Modelos do banco (SQLAlchemy)
│   ├── schemas/       # Validação de dados (Pydantic)
│   ├── routers/       # Rotas da API
│   └── database/      # Conexão com PostgreSQL
│
├── main.py            # Inicialização da aplicação FastAPI
├── Dockerfile         # Configuração da imagem Docker
├── docker-compose.yml # Orquestração dos containers
└── requirements.txt   # Dependências do projeto


## Arquitetura com Docker


Client
   │
   ▼
┌──────────────────────┐
│   Docker Container   │
│      FastAPI App     │
└──────────┬───────────┘
           │
           ▼
┌──────────────────────┐
│  Docker Container    │
│     PostgreSQL       │
└──────────────────────┘


## Rodando o projeto


Clone o repositório:
git clone https://github.com/seuuser/fastapi-docker-postgresql

Instale as dependências:
pip install -r requirements.txt

Execute a API:
uvicorn main:app --reload


## Rodando com Docker


docker compose up --build


## Documentação da API


Swagger UI:
http://127.0.0.1:8000/docs

ReDoc:
http://127.0.0.1:8000/redoc


## Objetivo


Este projeto foi desenvolvido para prática de desenvolvimento backend com FastAPI e uso de containers com Docker.
