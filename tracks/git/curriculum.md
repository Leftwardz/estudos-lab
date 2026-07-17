# Trilha: Git

Controle de versão distribuído — do básico ao fluxo profissional em equipe.

## Módulos

### Módulo 01 — Introdução ao Git
- O que é controle de versão
- Git vs outros VCS
- Instalação e configuração inicial (`user.name`, `user.email`)
- **Exercício:** Configurar Git e criar primeiro repositório com `git init`

### Módulo 02 — Commits e histórico
- Staging area (`git add`)
- Commits (`git commit`)
- Log (`git log`, `git log --oneline --graph`)
- **Exercício:** Fazer 5 commits em um projeto de texto

### Módulo 03 — Branches
- O que são branches
- Criar, listar e trocar (`git branch`, `git checkout`, `git switch`)
- **Exercício:** Criar branch `feature/login` e fazer commits nela

### Módulo 04 — Merge
- Fast-forward vs three-way merge
- Resolver conflitos básicos
- **Exercício:** Merge de `feature/login` em `main` com conflito simulado

### Módulo 05 — Remote e GitHub
- `git remote`, `git push`, `git pull`, `git fetch`
- Clonar repositórios
- **Exercício:** Publicar repositório no GitHub e clonar em outra pasta

### Módulo 06 — Fluxo Git Flow
- Branches `main`, `develop`, `feature`, `release`, `hotfix`
- Quando usar cada tipo
- **Exercício:** Simular feature branch completa com PR

### Módulo 07 — Rebase e cherry-pick
- `git rebase` interativo
- `git cherry-pick`
- Rebase vs merge
- **Exercício:** Rebase de feature branch e cherry-pick de um commit

### Módulo 08 — Stash e trabalho temporário
- `git stash`, `git stash pop`, `git stash list`
- Descartar mudanças (`git restore`, `git reset`)
- **Exercício:** Guardar trabalho incompleto, trocar de branch e recuperar

### Módulo 09 — Tags e releases
- Tags leves e anotadas
- `git tag`, versionamento semântico
- **Exercício:** Criar tag `v1.0.0` e push para remote

### Módulo 10 — Boas práticas e troubleshooting
- Mensagens de commit convencionais
- `.gitignore` avançado
- `git reflog`, recuperar commits perdidos
- **Exercício:** Recuperar commit "perdido" com reflog

## Critério de conclusão

Todos os 10 módulos marcados em `progress.md` com exercícios documentados em `sessoes/`.
