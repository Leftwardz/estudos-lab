# Curriculum — Cloud (Azure)

Azure aplicado. Repo de prática: **API + releases** das trilhas anteriores.

---

### Módulo 01 — Modelo mental (IaaS/PaaS/SaaS)

**Conceitos**
- IaaS, PaaS, SaaS — o que você gerencia vs o provedor
- Responsabilidade compartilhada
- Quando escolher cada modelo

**Exercício**
Classifique 5 serviços Azure (VM, App Service, Blob, Postgres flexível, Entra ID) em IaaS/PaaS/SaaS.

---

### Módulo 02 — Fundamentos Azure aplicados

**Conceitos**
- Resource Group, Subscription, Region
- Portal Azure e Azure CLI básico
- Naming conventions e tags

**Exercício**
Crie Resource Group via portal ou CLI; liste recursos com `az resource list`.

---

### Módulo 03 — Blob storage para artefatos/releases

**Conceitos**
- Storage Account, containers, blobs
- Upload de binários/releases
- URLs e acesso (SAS ou público controlado)

**Exercício**
Suba um artefato de release (zip) no Blob e gere URL de download.

---

### Módulo 04 — Banco gerenciado Postgres

**Conceitos**
- Azure Database for PostgreSQL (Flexible Server)
- Firewall, connection string
- Backup automático

**Exercício**
Provisione Postgres gerenciado e conecte a API (local ou container).

---

### Módulo 05 — Hospedar API (App Service / Container Apps)

**Conceitos**
- App Service vs Container Apps
- Deploy de imagem Docker
- Variáveis de ambiente na plataforma

**Exercício**
Deploy da API containerizada no App Service ou Container Apps.

---

### Módulo 06 — DNS e HTTPS

**Conceitos**
- Domínio customizado
- Certificado TLS (managed certificate)
- HTTPS obrigatório em produção

**Exercício**
Configure domínio (ou subdomínio Azure) com HTTPS na API hospedada.

---

### Módulo 07 — Secrets (Key Vault)

**Conceitos**
- Azure Key Vault para secrets
- DATABASE_URL, JWT_SECRET fora do código
- Referência de secrets no App Service

**Exercício**
Armazene JWT_SECRET no Key Vault e injete na API hospedada.

---

### Módulo 08 — Monitoramento e custo

**Conceitos**
- Application Insights / Log Analytics
- Alertas básicos
- Cost Management, budgets, tags para custo

**Exercício**
Ative logs/métricas na API; configure budget alert; documente custo estimado mensal.
