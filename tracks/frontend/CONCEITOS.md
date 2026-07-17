# Conceitos — Frontend

## Box Model

```
margin → border → padding → content
```

## Flexbox (resumo)

```css
.container {
  display: flex;
  justify-content: center;  /* eixo principal */
  align-items: center;      /* eixo cruzado */
  gap: 1rem;
}
```

## Grid (resumo)

```css
.grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1rem;
}
```

## DOM e eventos

```javascript
document.querySelector('#btn').addEventListener('click', () => {
  console.log('clicou');
});

const res = await fetch('/api/users');
const data = await res.json();
```

## Componentes (React)

```jsx
function Greeting({ name }) {
  const [count, setCount] = useState(0);
  return <button onClick={() => setCount(c => c + 1)}>{name}: {count}</button>;
}
```

## Acessibilidade (a11y)

- Use elementos semânticos (`<nav>`, `<main>`, `<button>`)
- Todo input precisa de `<label>` ou `aria-label`
- Contraste mínimo WCAG AA: 4.5:1 para texto normal
- Navegação por teclado deve funcionar

## Performance

- Code splitting e lazy loading de rotas
- Imagens: WebP, `loading="lazy"`, dimensões explícitas
- Evite re-renders desnecessários (memo, dependências corretas)
