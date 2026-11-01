# Blogester

Blog pessoal construído com **Astro**.

> Nicho e branding ainda em aberto — a estrutura técnica já está pronta.

## Stack

- [Astro](https://astro.build) 5
- Content Collections (Markdown / MDX)
- RSS + Sitemap
- CSS minimalista com variáveis (fácil de trocar no branding)

## Começar

```bash
npm install
npm run dev
```

Abra [http://localhost:4321](http://localhost:4321).

## Estrutura principal

```
src/
├── components/     # Header, Footer, BaseHead, etc.
├── content/
│   └── blog/       # Posts (.md / .mdx)
├── layouts/        # BaseLayout e BlogPost
├── pages/          # Rotas (index, blog, sobre, rss)
├── styles/         # global.css (tokens de design)
└── consts.ts       # Título, descrição e autor do site
```

## Adicionar um post

Crie um arquivo em `src/content/blog/meu-post.md`:

```md
---
title: 'Meu post'
description: 'Resumo'
pubDate: 2026-11-15
tags: ['exemplo']
---

Conteúdo aqui...
```

## Personalizar depois (branding)

1. `src/consts.ts` — nome, descrição e autor
2. `src/styles/global.css` — cores, fontes e tokens
3. `public/favicon.svg` — ícone
4. `astro.config.mjs` — `site:` com o domínio real

## Deploy

Funciona bem em:

- [Vercel](https://vercel.com)
- [Netlify](https://netlify.com)
- [Cloudflare Pages](https://pages.cloudflare.com)

```bash
npm run build
```

---

Feito para evoluir com calma: primeiro a base, depois o nicho e a marca.
