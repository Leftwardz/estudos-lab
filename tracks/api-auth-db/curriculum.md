# Curriculum — API + Auth + Banco

FastAPI, PostgreSQL, JWT. Repo de prática: **projeto API separado**.

---

### Módulo 01 — FastAPI Hello API

**Conceitos**
- App FastAPI, rota GET, Uvicorn
- Estrutura mínima de projeto Python

**Exercício**
Crie app com `GET /health` retornando `{"status": "ok"}`.

---

### Módulo 02 — Estrutura de projeto

**Conceitos**
- Separação: `routes`, `models`, `services`
- Injeção de dependências básica
- Organização escalável de pastas

**Exercício**
Reorganize o Hello API em pastas `routes/`, `models/`, `services/`.

---

### Módulo 03 — PostgreSQL + Docker

**Conceitos**
- Container PostgreSQL com Docker
- Variáveis de conexão (`DATABASE_URL`)
- Volume para persistência

**Exercício**
Suba Postgres via Docker e conecte a API (mesmo que só logando conexão ok).

---

### Módulo 04 — SQLAlchemy e modelos

**Conceitos**
- ORM, engine, session
- Modelos declarativos, tabelas
- Migrations (Alembic intro)

**Exercício**
Crie modelo `User` (id, email, password_hash) e gere tabela no banco.

---

### Módulo 05 — CRUD REST

**Conceitos**
- Endpoints REST para recurso
- Status HTTP corretos (200, 201, 404, 204)
- Path params e query params

**Exercício**
Implemente CRUD completo de um recurso (ex.: `items` ou `licenses`).

---

### Módulo 06 — Validação Pydantic

**Conceitos**
- Schemas request/response
- Validação automática, erros 422
- Separar schema de ORM model

**Exercício**
Crie schemas Pydantic para create/update/response do seu recurso.

---

### Módulo 07 — Endpoint core de negócio

**Conceitos**
- Regra de negócio na camada `services`
- Validação de licença/recurso (exemplo de domínio real)
- Erros de negócio vs erros técnicos

**Exercício**
Implemente endpoint que valida licença ou recurso (ex.: `POST /licenses/validate`).

---

### Módulo 08 — Autenticação JWT

**Conceitos**
- Registro e login com hash de senha (bcrypt)
- Access token JWT
- Dependency `get_current_user`

**Exercício**
Endpoints `/auth/register`, `/auth/login` e rota protegida `/me`.

---

### Módulo 09 — OpenAPI / Swagger

**Conceitos**
- Documentação automática FastAPI (`/docs`)
- Tags, descriptions, exemplos
- Bearer token no Swagger UI

**Exercício**
Documente todos os endpoints com tags, descrições e exemplo de auth.

---

### Módulo 10 — Testes Pytest

**Conceitos**
- `TestClient` do FastAPI
- Fixtures, banco de teste
- Testes de auth e CRUD

**Exercício**
Suite com pelo menos 5 testes cobrindo health, CRUD e login.

---

### Módulo 11 — Endpoint de releases/versões

**Conceitos**
- Versionamento de artefatos/releases
- Listagem e download metadata
- Integração futura com frontend e blob storage

**Exercício**
`GET /releases` listando versões; `GET /releases/{version}` com detalhes.

---

### Módulo 12 — Webhook de pagamento (mock)

**Conceitos**
- Webhooks: receber eventos externos
- Validação de payload, idempotência básica
- Atualizar estado no banco (ex.: licença ativa)

**Exercício**
`POST /webhooks/payment` com payload mock que ativa licença no banco.
