# Mehram Engineering Corporation, Ludhiana

Website for Mehram Engineering Corporation (est. 1976), Focal Point, Ludhiana: hose line end fittings and hose assemblies. Founded by the late S. Balbir Singh Mehram, run by S. Gurmehar Singh Mehram.

## Layout

- `public/mehramindustries/index.html` is the whole site: one static page, no build step.
- `wrangler.jsonc` deploys `public/` as a Cloudflare Workers static-assets site, routed at `harmanat.com/mehramindustries*` and on workers.dev.
- `public/_redirects` sends the bare workers.dev root to `/mehramindustries/`.

Pushes to `main` deploy automatically through Cloudflare Workers Builds.
