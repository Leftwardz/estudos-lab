# Curriculum — Banco Não Relacional

Foco: **quando usar** Postgres vs Redis vs Mongo.

---

### Módulo 01 — Árvore de decisão: Postgres vs Redis vs Mongo

**Conceitos**
- Postgres: dados relacionais, ACID, JOINs
- Redis: cache, filas, rate limit, TTL
- Mongo: documentos flexíveis, schema evolutivo
- Árvore de decisão por caso de uso

**Exercício**
Desenhe árvore de decisão (papel ou `sessoes/`). Para 5 cenários (sessão, cache, catálogo, fila, analytics), escolha a ferramenta e justifique.

---

### Módulo 02 — Relacional vs documento (teoria)

**Conceitos**
- Normalização vs desnormalização
- Embedding vs referencing (documentos)
- Consistência e transações

**Exercício**
Modele o mesmo domínio (ex.: blog ou e-commerce) em SQL normalizado e em documento Mongo — compare trade-offs.

---

### Módulo 03 — Redis na prática (cache)

**Conceitos**
- Strings, TTL, cache-aside
- Invalidação de cache
- Redis via Docker

**Exercício**
Adicione cache Redis em um endpoint da API (ex.: `GET /releases`).

---

### Módulo 04 — Rate limiting com Redis

**Conceitos**
- Contador por janela de tempo
- Proteção de endpoints sensíveis (login, webhook)
- Headers `X-RateLimit-*`

**Exercício**
Rate limit em `POST /auth/login` — ex.: 5 tentativas por minuto por IP.

---

### Módulo 05 — MongoDB intro

**Conceitos**
- Collections, documents, BSON
- CRUD básico
- Quando Mongo faz sentido (e quando não)

**Exercício**
Salve logs de eventos ou perfis flexíveis no Mongo; consulte com filtro simples.

---

### Módulo 06 — JSONB no Postgres (alternativa híbrida)

**Conceitos**
- Coluna JSONB no Postgres
- Query com operadores `->`, `->>`, `@>`
- Híbrido: relacional + flexível sem outro banco

**Exercício**
Adicione campo JSONB `metadata` em tabela existente; consulte por chave dentro do JSON.

---

### Módulo 07 — Projeto integrado + perguntas de entrevista

**Conceitos**
- Stack integrada: Postgres + Redis + (Mongo ou JSONB)
- Revisão da árvore de decisão
- Perguntas clássicas de entrevista sobre SQL vs NoSQL

**Exercício**
Documente arquitetura do seu projeto com justificativa por tecnologia. Responda 5 perguntas de entrevista sobre quando usar cada banco.
