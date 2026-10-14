# Mehram, Ludhiana

Website for the Mehram family companies in Focal Point, Ludhiana:

- Mehram Engineering Corporation (est. 1976): hose line end fittings and hose assemblies
- Mehram Industries (est. 1989): bicycle bottom bracket axles, cups, fittings and ball retainers

## Layout

- `public/mehramindustries/index.html` is the whole site: one static page, no build step.
- `wrangler.jsonc` deploys `public/` as a Cloudflare Workers static-assets site, routed at `harmanat.com/mehramindustries*` and on workers.dev.
- `public/_redirects` sends the bare workers.dev root to `/mehramindustries/`.
