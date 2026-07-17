# Trilha: DevOps

Integração contínua, containers e infraestrutura como código.

## Módulos

### Módulo 01 — Cultura e práticas DevOps
- CI/CD, feedback loops
- Infraestrutura como código
- **Exercício:** Mapear pipeline atual (ou ideal) de um projeto

### Módulo 02 — Docker fundamentos
- Imagens, containers, Dockerfile
- Volumes e networks
- **Exercício:** Containerizar app Node com multi-stage build

### Módulo 03 — Docker Compose
- Orquestração local de serviços
- **Exercício:** Stack app + PostgreSQL + Redis com compose

### Módulo 04 — CI com GitHub Actions
- Workflows, jobs, steps
- Cache e artifacts
- **Exercício:** Pipeline que roda lint e testes em cada PR

### Módulo 05 — CD e deploy automatizado
- Deploy em staging/produção
- Blue-green ou rolling deploy
- **Exercício:** Deploy automático após merge em `main`

### Módulo 06 — Kubernetes intro
- Pods, Deployments, Services
- kubectl básico
- **Exercício:** Deploy de app no minikube ou kind

### Módulo 07 — Terraform básico
- Providers, resources, state
- **Exercício:** Provisionar bucket S3 ou VM com Terraform

### Módulo 08 — Observabilidade
- Logs, métricas, traces
- Alertas básicos
- **Exercício:** Dashboard simples com Prometheus/Grafana ou equivalente

## Critério de conclusão

Pipeline CI/CD funcional, app containerizado e deploy documentado; 8 módulos em `progress.md`.
