This is a template portfolio website built with [Next.js](https://nextjs.org) (App Router) and TypeScript. It’s prewired for static export (GitHub Pages compatible) and easy customization via a single config file.

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Customize your template (one file)

All content (name, title, projects, research, certifications, contact, etc.) lives in `src/config/config.ts`.

Replace the placeholders with your own:

- `personal.name`: Put your name inside the quote
- `personal.title`: Your Title | Your Role
- `personal.tagline`: Short tagline
- `personal.location`: Your City, Country
- `seo.title` and `seo.description`: Your portfolio SEO
- `animatedText`: Words you want animated on the homepage
- `education`, `experience`, `projects`, `research`, `books`, `certifications`: Fill with your own entries. Keep the shapes the same.
- `contact`: Update email, LinkedIn, GitHub, Google Scholar, ORCID

Images are referenced via `getAsset()` which respects `NEXT_PUBLIC_BASE_PATH`. Replace the placeholder images with your own under `public/images/...`.

Optional: Set `NEXT_PUBLIC_BASE_PATH` in your environment or configure `basePath` in `next.config.ts` if deploying under a subpath (e.g., GitHub Pages).

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on GitHub Pages or Vercel

For GitHub Pages, ensure:

- `next.config.ts` sets `output: 'export'` and appropriate `basePath`/`assetPrefix`.
- Use a workflow to build and publish `./out`.

For Vercel, deploy directly; static export settings are optional.



---

## Notes

This repository is intended to be used as a template. Replace placeholders and remove sections you don’t need. If deploying under a subpath (e.g., GitHub Pages), set `NEXT_PUBLIC_BASE_PATH` and/or `basePath` in `next.config.ts` so all asset URLs resolve correctly.


