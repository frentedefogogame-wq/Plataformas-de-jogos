# Plataforma de Apps — Frente de Fogo

Site estático em HTML, CSS e JavaScript, hospedado no GitHub Pages.

## Estrutura

```
index.html                  Página inicial (lista de apps)
assets/
  css/style.css             Estilos
  js/apps.js                Catálogo de apps
  js/main.js                Renderização da lista
  js/game.js                Carregamento do jogo
apps/
  frente-de-fogo/
    index.html              Página do jogo
    build/                  Exportação Web da Godot 4 (index.html, .js, .wasm, .pck)
.nojekyll                   Desativa o Jekyll no GitHub Pages
```

## Como publicar no GitHub

1. Crie um repositório (ex.: `plataforma-frente-de-fogo`) e envie todos os arquivos.
2. Em **Settings > Pages**, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`.
3. O site ficará em `https://SEU-USUARIO.github.io/plataforma-frente-de-fogo/`.

## Como colocar o jogo

1. No Godot 4, use **Projeto > Exportar**, adicione o preset **Web** e desmarque **Threads**.
2. Exporte para `apps/frente-de-fogo/build/index.html`.
3. Envie a pasta `build/` para o repositório.

## Como adicionar outro app

1. Crie `apps/<nome-do-app>/index.html`.
2. Adicione um objeto em `assets/js/apps.js`.

## Pendências

- Aguardando os demais arquivos do Frente de Fogo para integração completa.
- Export Web da Godot ainda não foi testado nesta plataforma.
