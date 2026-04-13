# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
npm run dev      # Start development server at http://localhost:3000
npm run build    # Production build
npm run lint     # Run ESLint
```

There is no test suite configured yet.

## Architecture

This is a **Next.js 16 App Router** project with TypeScript and Tailwind CSS v4.

- `app/` — App Router directory. `layout.tsx` is the root layout (sets up Geist fonts, global CSS). `page.tsx` is the home route (`/`).
- `app/globals.css` — Global styles, Tailwind imports.
- `public/` — Static assets served at `/`.
- `@/*` path alias maps to the repo root.

Tailwind is configured via PostCSS (`postcss.config.mjs`) using the `@tailwindcss/postcss` plugin — there is no `tailwind.config.*` file; configuration is done in CSS.
