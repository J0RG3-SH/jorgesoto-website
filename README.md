# jorgesoto.es

Personal website — Jorge Soto, UX/Design/HCI Specialist.

## Deploy on GitHub Pages

1. Create a new repository on GitHub (e.g. `jorgesoto-website`)
2. Push this folder to the `main` branch
3. Go to **Settings → Pages**
4. Source: select **Deploy from a branch** → `main` / `/ (root)`
5. The `CNAME` file will auto-configure the custom domain

## DNS Configuration (at your domain registrar)

Add these records for `jorgesoto.es`:

### A Records (root domain)
| Type | Name | Value |
|------|------|-------|
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |

### CNAME Record (www subdomain)
| Type | Name | Value |
|------|------|-------|
| CNAME | www | YOUR_GITHUB_USERNAME.github.io |

Replace `YOUR_GITHUB_USERNAME` with your actual GitHub username.

### After DNS propagation (5 min – 24 hours)
- Go to repo **Settings → Pages → Custom domain**
- Enter `jorgesoto.es`
- Check **Enforce HTTPS**

## Files
- `index.html` — Main website (single page, bilingual EN/ES)
- `404.html` — Custom 404 error page
- `CNAME` — GitHub Pages custom domain config
- `.nojekyll` — Disables Jekyll processing
