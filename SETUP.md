# Setup — estudos-lab

## Clone e abrir no Cursor

```bash
git clone https://github.com/Leftwardz/estudos-lab.git
cd estudos-lab
```

1. Abra a pasta `estudos-lab` no Cursor (**File → Open Folder**)
2. A regra `estudos.mdc` entra em modo ensino automaticamente
3. Comece pelo índice: [tracks/README.md](tracks/README.md)

## Publicar alterações (progresso, anotações)

```bash
git add tracks/<trilha>/progress.md CONCEITOS.md sessoes/
git commit -m "Estudos: conclui módulo NN da trilha X"
git push origin main
```

Trabalhe direto na `main` — este repo é seu caderno de estudos.

## Estrutura esperada

```
estudos-lab/
├── README.md
├── FOCO.md
├── CONCEITOS.md
├── SETUP.md
├── .gitignore
├── .cursor/rules/estudos.mdc
├── sessoes/_TEMPLATE.md
├── templates/nova-trilha/
└── tracks/
    ├── README.md          ← índice principal
    └── <trilha>/          ← README + curriculum + progress
```

## Projetos de prática (fora deste repo)

| Trilha | Repo sugerido |
|--------|---------------|
| git | `git-sandbox` |
| api-auth-db | projeto API FastAPI separado |
| frontend | projeto web React separado |
| devops / cloud | mesma API ou derivado dela |
| banco-nao-relacional | API + Redis + Mongo conforme módulo |

## Pré-requisitos por trilha

| Ferramenta | Trilhas |
|------------|---------|
| Git 2.30+ | todas |
| Node 20+ | frontend |
| Python 3.11+ | api-auth-db |
| Docker | api-auth-db, devops, banco-nao-relacional |
| Conta Azure (free tier) | cloud |

## Convenção de sessões

Copie [sessoes/_TEMPLATE.md](sessoes/_TEMPLATE.md) para:

```
sessoes/YYYY-MM-DD-<trilha>-modulo-NN.md
```

Ao terminar, diga: **"Fim da sessão — atualiza progresso"**
