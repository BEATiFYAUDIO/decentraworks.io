# Decentraworks Static Site

This is a static export of `decentraworks.io`, cleaned for direct hosting without WordPress/Elementor.

## Local preview

```bash
python3 -m http.server 8787
# open http://localhost:8787
```

## Deploy options

### Option A: Cloudflare Pages (recommended)
1. Create a new GitHub repo and push this folder.
2. In Cloudflare Pages, connect the repo.
3. Build command: *(none)*
4. Output directory: `/`
5. Set custom domain: `decentraworks.io` and `www.decentraworks.io`.

### Option B: GitHub Pages
1. Push this folder to a repo.
2. Enable GitHub Pages from `main` branch, root folder.
3. Point DNS to GitHub Pages records.

## Notes
- Query-style WordPress links were normalized to clean routes:
  - `/identity/`
  - `/nft-marketplace/`
  - `/wallet/`
  - `/streaming/`
- Cloudflare anti-bot injected script blocks were removed from the static homepage.
