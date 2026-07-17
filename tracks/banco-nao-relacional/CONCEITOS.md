# Conceitos — Banco Não Relacional

## Tipos de NoSQL

| Tipo | Exemplo | Caso de uso |
|------|---------|-------------|
| Documento | MongoDB | Catálogos, perfis, CMS |
| Chave-valor | Redis, DynamoDB | Cache, sessões |
| Coluna | Cassandra | Time series, big data |
| Grafo | Neo4j | Redes sociais, recomendações |

## SQL vs NoSQL (quando usar)

| SQL | NoSQL |
|-----|-------|
| Relações complexas, JOINs | Schema flexível ou hierárquico |
| ACID forte | Escala horizontal prioritária |
| Dados estruturados e estáveis | Alto volume de escrita/leitura |

## Documento MongoDB (exemplo)

```json
{
  "_id": ObjectId("..."),
  "email": "user@example.com",
  "profile": {
    "name": "Ana",
    "tags": ["dev", "cloud"]
  },
  "createdAt": ISODate("2026-01-15")
}
```

## Embedding vs Referencing

| Embedding | Referencing |
|-----------|-------------|
| Dados lidos juntos | Dados grandes ou compartilhados |
| 1:few | 1:many, many:many |
| Ex.: endereço no user | Ex.: posts do autor |

## Redis — estruturas

```bash
SET user:1:name "Ana"
HSET user:1 email "ana@mail.com" role "admin"
EXPIRE session:abc 3600
LPUSH queue:jobs "job-1"
```

## Cache-aside

1. App busca no cache
2. Miss → busca no DB → grava no cache
3. Write → invalida ou atualiza cache

## CAP Theorem

Em partição de rede, escolha entre:
- **C**onsistency
- **A**vailability
- **P**artition tolerance (sempre necessário em sistemas distribuídos)

MongoDB: CP por padrão (consistência forte em replica set primário)
