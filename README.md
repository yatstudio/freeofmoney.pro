# freeofmoney.pro

Astro + GitHub Pages starter for `freeofmoney.pro`.

## Run locally

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
```

## Deploy to GitHub Pages

1. Push this repo to GitHub.
2. In GitHub repo settings, enable `Pages` and set source to `GitHub Actions`.
3. Keep `public/CNAME` as `freeofmoney.pro`.
4. DNS at your domain provider:
   - `A` records to GitHub Pages IPs:
     - `185.199.108.153`
     - `185.199.109.153`
     - `185.199.110.153`
     - `185.199.111.153`
   - Optional `AAAA` records:
     - `2606:50c0:8000::153`
     - `2606:50c0:8001::153`
     - `2606:50c0:8002::153`
     - `2606:50c0:8003::153`
   - `www` CNAME to `<your-github-username>.github.io`

## Structure

- `src/pages/index.astro`: homepage
- `src/pages/404.astro`: custom 404
- `src/layouts/BaseLayout.astro`: shared layout
- `src/styles/global.css`: global style
- `.github/workflows/deploy.yml`: CI deploy
- `public/CNAME`: custom domain
