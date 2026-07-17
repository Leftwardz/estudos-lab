# Curriculum — Git

Git profissional (fluxo empresa). Repo de prática: **git-sandbox**.

---

### Módulo 01 — Repositório e primeiro fluxo

**Conceitos**
- Clone, working directory, staging, commit
- Remote, push, pull
- Histórico básico (`git log`)

**Exercício**
No `git-sandbox`: clone (ou `git init`), crie um arquivo, faça commit e push para o GitHub.

---

### Módulo 02 — Branches no dia a dia

**Conceitos**
- Branch como linha de trabalho isolada
- `git switch` / `git checkout`, criar e listar branches
- Trabalhar em feature sem afetar `main`

**Exercício**
Crie `feature/minha-alteracao`, faça 2 commits e volte para `main` sem merge ainda.

---

### Módulo 03 — Pull Request no GitHub

**Conceitos**
- PR como revisão de código antes do merge
- Review, comentários, aprovação
- Squash merge vs merge commit

**Exercício**
Abra PR da sua branch para `main`, peça review (ou simule), faça squash merge.

---

### Módulo 04 — Conventional Commits

**Conceitos**
- Prefixos: `feat`, `fix`, `chore`, `docs`, `refactor`, `test`
- Mensagem no imperativo, corpo opcional
- Changelog e automação a partir de commits

**Exercício**
Reescreva ou faça 5 commits no `git-sandbox` seguindo Conventional Commits.

---

### Módulo 05 — Conflitos de merge

**Conceitos**
- Por que conflitos acontecem
- Marcadores `<<<<<<<`, `=======`, `>>>>>>>`
- Resolver manualmente e concluir merge

**Exercício**
Simule conflito (duas branches editando a mesma linha), resolva e complete o merge.

---

### Módulo 06 — Rebase interativo básico

**Conceitos**
- Rebase vs merge (histórico linear)
- `git rebase -i` para squash e reordenar commits
- Quando **não** rebasear (branch pública compartilhada)

**Exercício**
Use rebase interativo para juntar 3 commits pequenos em 1 commit `feat:` coerente.

---

### Módulo 07 — Desfazer mudanças

**Conceitos**
- `git restore` (working tree / staging)
- `git reset` (soft, mixed, hard)
- `git revert` (commit que desfaz outro)
- `git reflog` para recuperar commits "perdidos"

**Exercício**
Crie cenários de erro e recupere usando restore, revert e reflog.

---

### Módulo 08 — Tags e releases (semver)

**Conceitos**
- Tags leves vs anotadas
- Versionamento semântico (MAJOR.MINOR.PATCH)
- Release no GitHub a partir de tag

**Exercício**
Crie tag `v1.0.0`, push da tag e publique release no GitHub.

---

### Módulo 09 — Gitignore e arquivos sensíveis

**Conceitos**
- O que nunca commitar (.env, chaves, credenciais)
- Padrões em `.gitignore`
- Remover arquivo já rastreado (`git rm --cached`)

**Exercício**
Configure `.gitignore` no `git-sandbox`; simule commit acidental de `.env` e corrija.

---

### Módulo 10 — Simulação de entrevista

**Conceitos**
- Fluxo completo: issue → branch → PR → review → merge → tag → deploy
- Comunicação com o time (status, blockers)
- Perguntas comuns em entrevistas sobre Git

**Exercício**
Explique em voz alta (ou por escrito em `sessoes/`) o fluxo feature → produção. Responda 5 perguntas de entrevista sobre Git.
