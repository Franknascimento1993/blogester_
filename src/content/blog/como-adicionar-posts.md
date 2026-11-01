---
title: 'Como adicionar novos posts'
description: 'Guia rápido para criar artigos no blog.'
pubDate: 2026-11-01
tags: ['guia', 'markdown']
---

Para criar um novo post:

1. Crie um arquivo `.md` ou `.mdx` em `src/content/blog/`
2. Preencha o frontmatter:

```md
---
title: 'Título do post'
description: 'Resumo curto para SEO e listagens'
pubDate: 2026-11-15
tags: ['tag1', 'tag2']
draft: false
---
```

3. Escreva o conteúdo em Markdown abaixo do frontmatter.

Campos opcionais:

- `updatedDate` — data de atualização
- `heroImage` — caminho da imagem de capa (ex: `/images/capa.jpg`)
- `draft: true` — post não aparece nas listagens nem no RSS
