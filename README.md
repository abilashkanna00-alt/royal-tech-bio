# Royal Tech Bio — Complete Crop Solution

Official website for **Royal Tech Bio**, offering agricultural crop-care solutions and nutrition products for farmers. Based in Pollachi, Tamil Nadu, India.

---

## Tech Stack

- **Framework:** React 19 + TanStack Start + TanStack Router
- **Styling:** Tailwind CSS v4 + Radix UI Primitives + Lucide React
- **Build System:** Vite 8 + Nitro
- **Deployment Target:** Static Hosting (GitHub Pages, Cloudflare Pages, Vercel, Netlify)

---

## Local Development

Ensure you have Node.js 20+ installed.

```bash
# 1. Install dependencies
npm install

# 2. Run local development server
npm run dev

# 3. Run unit & routing tests
npm run test

# 4. Check TypeScript types
npx tsc --noEmit

# 5. Lint and format code
npm run lint
npm run format
```

---

## Production Build & Static Export

The project prerenders static HTML files for all routes and outputs a zero-server static bundle into `.output/public`:

```bash
# Build for apex domain or custom domain (default base path: /)
npm run build

# Or build for a repository-based GitHub Pages subpath:
BASE_PATH="/<your-repo-name>/" npm run build
```

The build process automatically generates:

- `index.html` (fully prerendered with hydration scripts)
- `404.html` (client-side routing fallback for GitHub Pages)
- `.nojekyll` (disables Jekyll processing on GitHub Pages)
- `sitemap.xml` and `robots.txt`

---

## Deploying to GitHub Pages

1. Push this repository to GitHub.
2. In your repository on GitHub, go to **Settings** > **Pages**.
3. Under **Build and deployment** > **Source**, choose **GitHub Actions**.
4. The automated workflow `.github/workflows/deploy.yml` will automatically detect your repository name, build the static assets, and deploy to your GitHub Pages URL (or custom domain).

### Connecting a Custom Domain

1. In GitHub, go to **Settings** > **Pages** > **Custom domain**.
2. Enter your domain (e.g., `royaltechbio.com`).
3. Point your DNS records (A/CNAME) to GitHub Pages as directed by GitHub.
4. The GitHub Actions workflow automatically adapts to the apex domain (`BASE_PATH=/`).
