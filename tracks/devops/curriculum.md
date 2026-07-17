# Curriculum — DevOps

Docker, CI/CD. Repo de prática: **API FastAPI** da trilha api-auth-db.

---

### Módulo 01 — Docker conceitos

**Conceitos**
- Imagem vs container
- Camadas, registry (Docker Hub)
- Quando containerizar vs rodar local

**Exercício**
Explique com suas palavras imagem, container e Dockerfile. Rode `docker run hello-world`.

---

### Módulo 02 — Dockerfile da API

**Conceitos**
- `FROM`, `WORKDIR`, `COPY`, `RUN`, `CMD`/`ENTRYPOINT`
- Multi-stage build (opcional)
- `.dockerignore`

**Exercício**
Escreva Dockerfile que sobe a API FastAPI na porta 8000.

---

### Módulo 03 — docker-compose (api + postgres)

**Conceitos**
- Serviços, networks, volumes
- `depends_on`, variáveis de ambiente entre serviços
- Desenvolvimento local com um comando

**Exercício**
`docker compose up` sobe API + PostgreSQL funcionando juntos.

---

### Módulo 04 — Ambientes e .env

**Conceitos**
- `.env` para dev vs prod
- Nunca commitar secrets
- `env_file` no Compose

**Exercício**
Configure `.env.example` e documente variáveis necessárias.

---

### Módulo 05 — CI testes (GitHub Actions)

**Conceitos**
- Workflow em `.github/workflows/`
- Trigger em push/PR
- Rodar pytest no CI

**Exercício**
Pipeline que executa testes da API em cada PR.

---

### Módulo 06 — CI lint opcional

**Conceitos**
- Linter (ruff, flake8 ou eslint conforme stack)
- Falhar build se lint quebrar
- Cache de dependências no CI

**Exercício**
Adicione step de lint no workflow (pode ser warning-only no início).

---

### Módulo 07 — Build de imagem no CI

**Conceitos**
- `docker build` no GitHub Actions
- Tags por branch/commit
- Push para registry (GHCR ou Docker Hub)

**Exercício**
CI constrói imagem Docker da API e publica no registry.

---

### Módulo 08 — Deploy manual documentado

**Conceitos**
- Deploy manual como primeiro passo antes de CD automático
- Checklist: migrate, env, health check
- Rollback básico

**Exercício**
Documente em `sessoes/` passo a passo de deploy manual da API containerizada.
