# Arise - Agent Instructions

## Project Overview

Astro v4.3.2 personal CV/portfolio website. Data-driven from `cv.json` (jsonresume.org schema). Single-page app, designed for both web and print/PDF output.

## Key Commands

- **Dev server:** `npm run dev` → http://localhost:4321/
- **Build:** `npm run build` (runs `astro check && astro build`)
- **Preview:** `npm run preview`

## Architecture

- **Entry point:** `src/pages/index.astro`
- **Data source:** `cv.json` (root) — all CV content comes from here
- **Type definitions:** `src/cv.d.ts` (CV interface), `src/types.d.ts` (SocialIcon)
- **Components:** `src/components/sections/` (Hero, About, Experience, Education, Certificates, Projects, Skills)
- **Layouts:** `src/layouts/Layout.astro`
- **Path aliases:** `@cv` → `./cv.json`, `@/*` → `src/*`

## Development Notes

- No ESLint/Prettier configured — follow existing code style
- TypeScript strict mode (extends `astro/tsconfigs/strict`)
- Content in Spanish (site language)
- Print styles use `.print` / `.no-print` CSS classes
- `mailtoui` library handles email links (loaded in Hero component)

## Build & Deploy

- Build output goes to `./dist`
- `.astro/` directory contains generated types (gitignored)
- Deploy via Git push → Jenkins or FTP (per README)

## Common Pitfalls

- Editing content? Modify `cv.json`, not the components directly
- New CV sections? Update both `cv.json` AND `src/cv.d.ts` types
- Adding social networks? Add icon in `src/icons/`, map in `Hero.astro`'s `SOCIAL_ICONS`
