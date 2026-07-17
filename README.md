# estudos-lab

Repositório de **estudos** — trilhas flexíveis, progresso em Markdown. Você alterna conforme o humor; o agente guia em modo ensino.

## Como usar com o Cursor

1. Abra esta pasta no Cursor (a regra `.cursor/rules/estudos.mdc` ativa o modo ensino)
2. Veja o índice em [tracks/README.md](tracks/README.md)
3. Opcional: preencha [FOCO.md](FOCO.md) com a trilha do dia
4. Diga ao agente, por exemplo:
   - *"Quais estudos temos no foco?"*
   - *"Hoje git módulo 3"*
   - *"Fim da sessão — atualiza progresso"*

## Modo de trabalho

- **Você codifica primeiro** — o agente orienta, revisa e faz perguntas
- Projetos de prática ficam em **repos separados** (ex.: `git-sandbox`, API, web)
- Este repo guarda trilhas, progresso e anotações de sessão

## Trilhas (55 módulos)

| Trilha | Módulos | Foco |
|--------|---------|------|
| [git](tracks/git/) | 10 | Git profissional, fluxo em empresa |
| [api-auth-db](tracks/api-auth-db/) | 12 | FastAPI, PostgreSQL, JWT |
| [frontend](tracks/frontend/) | 10 | React + Vite |
| [devops](tracks/devops/) | 8 | Docker, CI/CD |
| [cloud](tracks/cloud/) | 8 | Azure |
| [banco-nao-relacional](tracks/banco-nao-relacional/) | 7 | Quando usar Postgres, Redis ou Mongo |

## Arquivos úteis

| Arquivo | Uso |
|---------|-----|
| [SETUP.md](SETUP.md) | Clone, push, abrir no Cursor |
| [FOCO.md](FOCO.md) | Trilha e humor do dia (opcional) |
| [CONCEITOS.md](CONCEITOS.md) | O que você já aprendeu (por trilha) |
| [sessoes/_TEMPLATE.md](sessoes/_TEMPLATE.md) | Modelo de anotação de sessão |

## Workflow Git deste repo

- Trabalhe direto na `main`
- Commits claros após sessões
- Atualize `progress.md` e `CONCEITOS.md` ao estudar
