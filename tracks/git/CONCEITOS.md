# Conceitos — Git

Glossário de referência rápida para a trilha Git.

## Termos fundamentais

| Termo | Definição |
|-------|-----------|
| **Repositório** | Diretório versionado pelo Git, contém `.git/` |
| **Commit** | Snapshot imutável do projeto em um ponto no tempo |
| **Branch** | Linha independente de desenvolvimento |
| **HEAD** | Ponteiro para o commit/branch atual |
| **Staging area** | Área intermediária antes do commit (`git add`) |
| **Remote** | Repositório hospedado em outro lugar (ex.: GitHub) |

## Comandos essenciais

```bash
git init                    # Inicia repositório
git status                  # Estado do working tree
git add <arquivo>           # Adiciona ao staging
git commit -m "mensagem"    # Cria commit
git log --oneline --graph   # Histórico visual
git branch <nome>         # Cria branch
git switch <branch>         # Troca de branch
git merge <branch>          # Integra branch
git push origin <branch>    # Envia para remote
git pull                    # Busca e integra do remote
```

## Fluxos de trabalho

- **Trunk-based:** commits diretos ou PRs curtos em `main`
- **Git Flow:** branches longas (`develop`, `feature/*`, `release/*`)
- **GitHub Flow:** branch de feature → PR → merge em `main`

## Resolução de conflitos

1. Git marca arquivos com `<<<<<<<`, `=======`, `>>>>>>>`
2. Edite manualmente escolhendo o código correto
3. `git add` nos arquivos resolvidos
4. `git commit` (ou continue o merge/rebase)

## Boas práticas

- Commits pequenos e atômicos
- Mensagens no imperativo: "Adiciona validação de email"
- Nunca force push em branches compartilhadas sem combinar
- Use `.gitignore` desde o primeiro commit
