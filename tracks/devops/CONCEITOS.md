# Conceitos — DevOps

## CI vs CD

| | CI (Integração Contínua) | CD (Entrega/Deploy Contínuo) |
|---|--------------------------|------------------------------|
| Foco | Build e testes automáticos | Deploy automático em ambientes |
| Gatilho | Push, PR | Merge em branch de release |

## Docker

```dockerfile
# Multi-stage example
FROM node:20-alpine AS build
WORKDIR /app
COPY package*.json ./
RUN npm ci
COPY . .
RUN npm run build

FROM node:20-alpine
WORKDIR /app
COPY --from=build /app/dist ./dist
CMD ["node", "dist/index.js"]
```

## Docker Compose

```yaml
services:
  app:
    build: .
    ports: ["3000:3000"]
    depends_on: [db]
  db:
    image: postgres:15
    environment:
      POSTGRES_PASSWORD: secret
```

## Kubernetes (objetos principais)

| Objeto | Função |
|--------|--------|
| Pod | Menor unidade executável |
| Deployment | Gerencia réplicas de pods |
| Service | Expõe pods na rede |
| Ingress | Roteamento HTTP externo |

## GitHub Actions (estrutura)

```yaml
name: CI
on: [push, pull_request]
jobs:
  test:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - run: npm ci && npm test
```

## Observabilidade (três pilares)

1. **Logs** — eventos discretos (JSON estruturado)
2. **Métricas** — números agregados ao longo do tempo
3. **Traces** — fluxo de uma request entre serviços

## IaC (Infrastructure as Code)

- Estado declarativo versionado em Git
- `terraform plan` antes de `apply`
- Nunca editar infra manualmente em produção
