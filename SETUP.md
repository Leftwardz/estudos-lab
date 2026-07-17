# Setup do Laboratório de Estudos

Guia para configurar o ambiente e começar a estudar nas trilhas.

## Pré-requisitos

| Ferramenta | Versão mínima | Verificar |
|------------|---------------|-----------|
| Git        | 2.30+         | `git --version` |
| Node.js    | 20 LTS        | `node --version` |
| Docker     | 24+           | `docker --version` |
| Docker Compose | 2.20+     | `docker compose version` |

### Opcionais por trilha

| Trilha | Ferramentas extras |
|--------|--------------------|
| api-auth-db | PostgreSQL 15+, Postman ou Insomnia |
| frontend | npm ou pnpm |
| devops | kubectl, Terraform |
| cloud | Conta AWS/GCP/Azure (free tier) |
| banco-nao-relacional | MongoDB, Redis |

## Instalação rápida

```bash
# Clonar o repositório
git clone https://github.com/Leftwardz/estudos-lab.git
cd estudos-lab

# Verificar estrutura
ls tracks/
```

## Como estudar

1. Escolha uma trilha em `tracks/README.md`
2. Leia `curriculum.md` da trilha para ver os módulos
3. Consulte `CONCEITOS.md` antes de cada módulo
4. Use `FOCO.md` para saber o objetivo da sessão
5. Registre avanço em `progress.md`
6. Salve anotações e exercícios em `sessoes/`

## Estrutura de pastas

```
estudos-lab/
├── SETUP.md                 # Este arquivo
├── tracks/
│   ├── README.md            # Índice das trilhas
│   ├── git/
│   ├── api-auth-db/
│   ├── frontend/
│   ├── devops/
│   ├── cloud/
│   └── banco-nao-relacional/
├── sessoes/                 # Anotações e exercícios por data
└── .cursor/rules/
    └── estudos.mdc          # Regras do Cursor para estudos
```

## Convenção de sessões

Crie arquivos em `sessoes/` com o formato:

```
sessoes/YYYY-MM-DD-<trilha>-modulo-NN.md
```

Exemplo: `sessoes/2026-07-17-git-modulo-01.md`

## Dicas

- Estude um módulo por sessão; marque como concluído em `progress.md`
- Faça commits pequenos ao praticar exercícios
- Use branches para experimentos: `estudo/<trilha>-modulo-NN`
