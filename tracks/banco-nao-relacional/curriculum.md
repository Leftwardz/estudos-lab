# Trilha: Banco Não Relacional

NoSQL, bancos de documentos, cache e modelagem orientada a dados.

## Módulos

### Módulo 01 — SQL vs NoSQL
- Quando usar relacional vs não relacional
- Tipos: documento, chave-valor, coluna, grafo
- **Exercício:** Comparar mesmo domínio modelado em SQL e documento

### Módulo 02 — MongoDB fundamentos
- Collections, documents, BSON
- CRUD básico
- **Exercício:** Inserir e consultar documentos de usuários

### Módulo 03 — Queries e índices no MongoDB
- Filtros, projeção, sort, limit
- Índices simples e compostos
- **Exercício:** Queries com `explain()` e criação de índices

### Módulo 04 — Modelagem de documentos
- Embedding vs referencing
- Padrões de schema design
- **Exercício:** Modelar blog (posts, comentários, autores)

### Módulo 05 — Redis e cache
- Strings, hashes, lists, sets
- TTL e estratégias de cache (cache-aside)
- **Exercício:** Cache de API com Redis

### Módulo 06 — Agregações MongoDB
- Pipeline: `$match`, `$group`, `$lookup`
- **Exercício:** Relatório de vendas por categoria com aggregation

### Módulo 07 — Consistência e escalabilidade
- CAP theorem, eventual consistency
- Sharding e replica sets (conceito)
- **Exercício:** Documentar trade-offs de um cenário multi-região

## Critério de conclusão

App usando MongoDB e Redis com modelagem documentada; 7 módulos em `progress.md`.
