# Curriculum — Frontend (React)

React + Vite. Repo de prática: **projeto web separado**.

---

### Módulo 01 — Vite + React

**Conceitos**
- Scaffold com Vite (`npm create vite@latest`)
- Estrutura de pastas, `main.jsx`, componente raiz
- Dev server e hot reload

**Exercício**
Crie app Vite + React e exiba "Hello" na tela.

---

### Módulo 02 — Componentes e props

**Conceitos**
- Componentes funcionais
- Props tipadas (ou PropTypes)
- Composição de componentes

**Exercício**
Crie `Header`, `Card` e `Button` reutilizáveis com props.

---

### Módulo 03 — useState e formulários

**Conceitos**
- Estado local com `useState`
- Controlled inputs
- Submit de formulário

**Exercício**
Formulário de login (email + senha) sem integrar API ainda.

---

### Módulo 04 — useEffect e fetch

**Conceitos**
- `useEffect` para side effects
- `fetch` para API pública ou mock
- Loading state básico

**Exercício**
Busque lista de dados (mock ou API pública) e renderize em lista.

---

### Módulo 05 — Login JWT

**Conceitos**
- POST login, receber token
- Armazenar token (localStorage ou memória)
- Redirecionar após login

**Exercício**
Integre formulário de login com `/auth/login` da sua API.

---

### Módulo 06 — React Router (rotas protegidas)

**Conceitos**
- `react-router-dom`, rotas e navegação
- Rota privada: redireciona se não autenticado
- Layout com outlet

**Exercício**
Rotas `/login`, `/dashboard` (protegida) e `/releases`.

---

### Módulo 07 — Chamadas autenticadas

**Conceitos**
- Header `Authorization: Bearer <token>`
- Wrapper ou interceptor de fetch
- Tratar 401 (logout)

**Exercício**
Chame `GET /me` autenticado e exiba dados do usuário.

---

### Módulo 08 — Página de download/releases

**Conceitos**
- Consumir `GET /releases`
- Listar versões, link de download
- Integração com API do módulo 11 da trilha api-auth-db

**Exercício**
Página `/releases` listando versões da API.

---

### Módulo 09 — UX (loading, erro)

**Conceitos**
- Estados: loading, error, empty, success
- Feedback visual (spinner, mensagem de erro)
- Desabilitar botão durante submit

**Exercício**
Adicione loading e tratamento de erro em login e lista de releases.

---

### Módulo 10 — Build e deploy estático

**Conceitos**
- `npm run build`, pasta `dist/`
- Variáveis de ambiente (`VITE_API_URL`)
- Deploy estático (GitHub Pages, Azure Static Web Apps, etc.)

**Exercício**
Gere build de produção e documente passos de deploy estático.
