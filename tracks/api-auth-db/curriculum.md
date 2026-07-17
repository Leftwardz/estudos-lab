# Trilha: API, Auth e Banco de Dados

Construção de APIs REST com autenticação, autorização e persistência em banco relacional.

## Módulos

### Módulo 01 — Fundamentos de HTTP
- Métodos (GET, POST, PUT, PATCH, DELETE)
- Status codes, headers, body
- **Exercício:** Testar endpoints públicos com curl

### Módulo 02 — REST e design de APIs
- Recursos, URIs, idempotência
- Versionamento e paginação
- **Exercício:** Desenhar API de um CRUD de tarefas (OpenAPI ou markdown)

### Módulo 03 — Primeira API com Node/Express
- Rotas, middleware, JSON
- **Exercício:** API `/health` e CRUD em memória

### Módulo 04 — Banco relacional e SQL
- Tabelas, chaves primárias e estrangeiras
- SELECT, INSERT, UPDATE, DELETE
- **Exercício:** Criar schema `users` e `tasks` no PostgreSQL

### Módulo 05 — ORM e migrations
- Prisma ou TypeORM
- Migrations up/down
- **Exercício:** Conectar API ao PostgreSQL com migrations

### Módulo 06 — Validação e tratamento de erros
- Validação de entrada (Zod, Joi)
- Middleware de erro centralizado
- **Exercício:** Validar body de POST `/users`

### Módulo 07 — Autenticação com JWT
- Login, registro, hash de senha (bcrypt)
- Access token e refresh token
- **Exercício:** Endpoints `/auth/register` e `/auth/login`

### Módulo 08 — Autorização e RBAC
- Roles (admin, user)
- Middleware de permissão
- **Exercício:** Rotas admin protegidas por role

### Módulo 09 — Sessões e cookies
- HttpOnly cookies vs Bearer token
- CSRF básico
- **Exercício:** Login com cookie de sessão

### Módulo 10 — Testes de API
- Testes de integração com supertest
- Fixtures e banco de teste
- **Exercício:** Suite de testes para auth e CRUD

### Módulo 11 — Documentação OpenAPI
- Swagger UI
- Schemas e exemplos
- **Exercício:** Documentar API completa em `/docs`

### Módulo 12 — Deploy e variáveis de ambiente
- `.env`, secrets, 12-factor app
- Health check e graceful shutdown
- **Exercício:** Containerizar API com Docker

## Critério de conclusão

API funcional com auth, banco PostgreSQL, testes e documentação; 12 módulos em `progress.md`.
