# madeforthe.net — Landing Page

Peter Thomas's personal landing page, deployed to madeforthe.net via Cloudflare Workers.

## Stack
- Astro v5 (static output)
- Single page — all styles inline in `src/pages/index.astro`
- Tailwind CDN + custom theme (bg, ink, muted, rule, navy)
- No external dependencies (Google Fonts loaded via link tag)
- Deployed to Cloudflare Workers with static assets

## Local development
```bash
npm run dev
```

## Build
```bash
npm run build
```

Output goes to `dist/`.

## Deploy
Not yet set up. Will use GitHub Actions + `wrangler deploy` (same pattern as cv/ project).

Cloudflare Worker name: `madeforthe`
Cloudflare account ID: `b327ad19653b5a65225b5edd2cfe144c`

## Custom domain
Will be pointed to `madeforthe.net` (root domain) via Cloudflare Workers custom domain.
DNS for madeforthe.net is managed in Cloudflare.

## Notes
- `/cv` link points to cv.madeforthe.net (separate Workers project)
- Deploy workflow not yet created — user wants to tweak content before going live
