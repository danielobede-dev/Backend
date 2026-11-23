# estudos-backend 🐍

Registro da minha transição de desenvolvedor frontend para backend com Python. Aqui ficam os exercícios, projetos e anotações de um plano de estudos de 16 semanas, do básico da linguagem até uma API em produção.

Venho do frontend (TypeScript/React). Este repositório documenta, commit a commit, como estou construindo a base de backend: APIs, banco de dados, testes, segurança e deploy.

# 🎯 Objetivo

Chegar a um nível em que eu consiga:

projetar e implementar APIs REST bem estruturadas;
modelar e consultar bancos relacionais com segurança e desempenho;
escrever testes automatizados confiáveis;
empacotar e publicar aplicações com Docker e CI/CD.
# 🧰 Stack
Área	Ferramentas
Linguagem	Python 3.12+
Dependências	uv
Qualidade	ruff (lint/format), mypy (tipos), pytest (testes)
API	FastAPI + Pydantic
Banco de dados	PostgreSQL, SQLAlchemy 2.0, Alembic
Infra	Docker, docker-compose, GitHub Actions
Extras	Redis, JWT, Celery/RQ
# 🗺️ Progresso
[ ] Fase 1 — Fundamentos de Python (semanas 1–4) Sintaxe, POO, type hints, async e ferramentas. Entregável: CLI que consome uma API pública, com testes.
[ ] Fase 2 — APIs e banco de dados (semanas 5–8) FastAPI, REST, SQL, SQLAlchemy e migrations. Entregável: API de tarefas com Postgres.
[ ] Fase 3 — Segurança, testes e infra (semanas 9–12) Autenticação JWT, pytest, Docker, OWASP e filas. Entregável: API autenticada, com mais de 80% de cobertura, subindo com docker compose up.
[ ] Fase 4 — Projeto final e deploy (semanas 13–16) Projeto fullstack, CI e deploy. Entregável: aplicação publicada com front consumindo a API.
# 📁 Estrutura
estudos-backend/
├── fase-1-fundamentos/      # exercícios e a CLI
├── fase-2-api-banco/        # API de tarefas (FastAPI + Postgres)
├── fase-3-seguranca-infra/  # auth, testes, Docker
├── projeto-final/           # projeto fullstack publicado
└── anotacoes/               # resumos e aprendizados por semana
# 🚀 Como rodar

Pré-requisitos: Python 3.12+, uv e Docker.

bash
# clonar o repositório
git clone https://github.com/<seu-usuario>/estudos-backend.git
cd estudos-backend

# instalar dependências
uv sync

# checar qualidade
uv run ruff check .
uv run mypy .
uv run pytest

Cada fase tem seu próprio README com instruções específicas (por exemplo, subir o banco com docker compose up).

# 🔁 Fluxo de trabalho

Mantenho o mesmo fluxo que uso no trabalho:

uma branch por tópico (feat/fase-2-jwt, study/sql-joins);
ruff, mypy e pytest passando antes de cada commit;
PR para a main com uma descrição do que aprendi.
📚 Referências principais
Tutorial oficial do Python (pt-BR)
Tutorial do FastAPI
Use The Index, Luke
SQLAlchemy 2.0 Tutorial
OWASP API Security Top 10

# 💬 Sugestões e dicas são bem-vindas: abra uma issue!
