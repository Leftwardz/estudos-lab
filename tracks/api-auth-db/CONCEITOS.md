# Conceitos — API, Auth e Banco de Dados

## HTTP

| Código | Significado | Uso comum |
|--------|-------------|-----------|
| 200 | OK | GET bem-sucedido |
| 201 | Created | POST criou recurso |
| 400 | Bad Request | Validação falhou |
| 401 | Unauthorized | Não autenticado |
| 403 | Forbidden | Sem permissão |
| 404 | Not Found | Recurso inexistente |
| 500 | Internal Error | Erro no servidor |

## REST

- **Recurso:** entidade exposta via URI (`/users/1`)
- **Representação:** JSON do recurso
- **Stateless:** cada request traz contexto necessário (token, etc.)

## Autenticação vs Autorização

| | Autenticação | Autorização |
|---|--------------|-------------|
| Pergunta | Quem é você? | O que pode fazer? |
| Exemplo | Login + JWT | Role `admin` |

## JWT (estrutura)

```
header.payload.signature
```

- **Access token:** curta duração (15min–1h)
- **Refresh token:** longa duração, usado para renovar access

## SQL essencial

```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  email VARCHAR(255) UNIQUE NOT NULL,
  password_hash VARCHAR(255) NOT NULL,
  created_at TIMESTAMPTZ DEFAULT NOW()
);

SELECT * FROM users WHERE email = $1;
INSERT INTO users (email, password_hash) VALUES ($1, $2);
```

## Segurança

- Nunca armazene senha em texto plano — use bcrypt/argon2
- Valide toda entrada do cliente
- Use HTTPS em produção
- Rate limiting em endpoints de login
