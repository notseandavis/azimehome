# azimehome

Static site served by GitHub Pages at https://azimehome.com.

- `index.html` – home page
- `404.html` – not-found page
- `CNAME` – custom domain for GitHub Pages
- `.nojekyll` – serve files as-is (skip Jekyll processing)

## One-time setup

1. **GitHub Pages:** Repo → Settings → Pages → Source: *Deploy from a branch*,
   Branch: `main`, folder `/ (root)`. Custom domain: `azimehome.com`.
2. **DNS** (at your domain registrar):
   - Apex `azimehome.com` – four `A` records:
     `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - Optional IPv6 – `AAAA` records:
     `2606:50c0:8000::153`, `2606:50c0:8001::153`, `2606:50c0:8002::153`, `2606:50c0:8003::153`
   - `www` – `CNAME` record pointing to `notseandavis.github.io`
3. Once DNS resolves and the certificate is issued, tick **Enforce HTTPS** in Settings → Pages.
