# Template — Nova trilha

Use esta pasta como modelo ao criar uma trilha customizada em `tracks/<nome>/`.

## Arquivos obrigatórios (3 por trilha)

```
tracks/<nome-da-trilha>/
├── README.md        # Visão geral e repo de prática sugerido
├── curriculum.md    # Módulos com Conceitos + Exercício
└── progress.md      # Tabela [ ] / [x] + Data
```

## README.md (trilha)

- Nome e objetivo da trilha
- Quantidade de módulos
- Repo ou ambiente de prática sugerido
- Link para `curriculum.md` e `progress.md`

## curriculum.md

Para cada módulo:

```markdown
### Módulo NN — Título

**Conceitos**
- ponto 1
- ponto 2

**Exercício**
Descrição clara do que o aluno deve fazer sozinho.
```

## progress.md

```markdown
| Módulo | Título | Concluído | Data |
|--------|--------|-----------|------|
| 01 | Título | [ ] | — |
```

## Depois de criar

1. Adicione a trilha em `tracks/README.md`
2. Adicione seção em `CONCEITOS.md` (raiz)
3. Atualize `.cursor/rules/estudos.mdc` se necessário
