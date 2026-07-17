# Índice das trilhas

Leia este arquivo quando perguntar: **"Quais estudos temos no foco?"**

Laboratório com 6 trilhas flexíveis — **a ordem não é obrigatória**. Alterne conforme seu humor e energia.

## Trilhas

| Trilha | Módulos | Tema | Links |
|--------|---------|------|-------|
| [git](./git/) | 10 | Git profissional (fluxo empresa) | [curriculum](./git/curriculum.md) · [progresso](./git/progress.md) |
| [api-auth-db](./api-auth-db/) | 12 | API REST, auth, banco relacional | [curriculum](./api-auth-db/curriculum.md) · [progresso](./api-auth-db/progress.md) |
| [frontend](./frontend/) | 10 | React | [curriculum](./frontend/curriculum.md) · [progresso](./frontend/progress.md) |
| [devops](./devops/) | 8 | Docker, CI/CD | [curriculum](./devops/curriculum.md) · [progresso](./devops/progress.md) |
| [cloud](./cloud/) | 8 | Cloud (Azure) | [curriculum](./cloud/curriculum.md) · [progresso](./cloud/progress.md) |
| [banco-nao-relacional](./banco-nao-relacional/) | 7 | Postgres vs Redis vs Mongo | [curriculum](./banco-nao-relacional/curriculum.md) · [progresso](./banco-nao-relacional/progress.md) |

**Total: 55 módulos**

## Ordem sugerida (não obrigatória)

```
git → api-auth-db → frontend → devops → cloud → banco-nao-relacional
```

Trilhas independentes (ex.: `git` e `frontend`) podem rodar em paralelo.

## Como marcar progresso

1. Estude o módulo seguindo `tracks/<trilha>/curriculum.md`
2. Ao concluir, marque `[x]` em `tracks/<trilha>/progress.md` com a data
3. Registre conceitos em [CONCEITOS.md](../CONCEITOS.md) (raiz)
4. Opcional: anote a sessão em `sessoes/` usando `_TEMPLATE.md`
5. Diga ao agente: **"Fim da sessão — atualiza progresso"**

## Arquivos por trilha (3)

| Arquivo | Conteúdo |
|---------|----------|
| `README.md` | Visão geral e repo de prática |
| `curriculum.md` | Módulos com **Conceitos** e **Exercício** |
| `progress.md` | Checklist `[ ]` / `[x]` por módulo |

## Foco do dia

Opcional: preencha [FOCO.md](../FOCO.md) na raiz com trilha, módulo e energia.
