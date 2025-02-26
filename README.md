# grid-template-areas

O `grid-template-areas` é uma propriedade do CSS Grid que permite nomear áreas dentro do grid, facilitando a organização e o posicionamento dos elementos.

## Como usar

1. Defina o container como `display: grid`.
2. Use `grid-template-areas` para criar um layout nomeado.
3. Atribua áreas aos elementos filhos com `grid-area`.

### Exemplo:

```css
.container {
  display: grid;
  grid-template-areas:
    "header header"
    "sidebar content"
    "footer footer";
  grid-template-columns: 200px 1fr;
  grid-template-rows: auto 1fr auto;
}

.header {
  grid-area: header;
  background: lightblue;
}

.sidebar {
  grid-area: sidebar;
  background: lightgray;
}

.content {
  grid-area: content;
  background: white;
}

.footer {
  grid-area: footer;
  background: lightcoral;
}



<div class="container">
  <header class="header">Header</header>
  <aside class="sidebar">Sidebar</aside>
  <main class="content">Content</main>
  <footer class="footer">Footer</footer>
</div>
