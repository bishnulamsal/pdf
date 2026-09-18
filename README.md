# PDF Tools — Static GitHub Pages Project

A complete browser-first PDF tools website built with HTML, CSS and vanilla JavaScript. No Node.js, npm, database or backend is required.

## Quick GitHub setup
1. Create a new GitHub repository.
2. Upload **all files and folders in this project root**. Do not upload the ZIP itself.
3. Commit to the `main` branch.
4. In **Settings → Pages**, select **GitHub Actions** as the source.
5. The included `.github/workflows/pages.yml` deploys the site automatically.

### Custom domain
If you want `pdf.bishnulamsal.com.np`, create a file named `CNAME` in the repository root containing exactly:

```text
pdf.bishnulamsal.com.np
```

Then point the DNS record for the subdomain to GitHub Pages according to GitHub's current Pages instructions.

## Structure
- `index.html` — homepage
- `tools/` — individual PDF tools
- `css/main.css` — shared design system
- `js/core.js` — theme/toast/progress utilities
- `js/file-utils.js` — file/drop/download helpers
- `js/pdf-engine.js` — PDF.js/pdf-lib integration
- `js/tools/app.js` — tool functionality
- `workers/` — worker entry point
- `.github/workflows/pages.yml` — automatic GitHub Pages deployment
- `.nojekyll` — prevents Jekyll processing
- `robots.txt`, `sitemap.xml`, `ads.txt` — deployment/SEO files

## External libraries
The site uses pinned browser CDN releases for pdf-lib, PDF.js, JSZip, FileSaver.js, Font Awesome, html2canvas and jsPDF. For production, self-host the libraries if you want the site to remain functional when a CDN is unavailable.

## Important limitations
- Protect PDF does not fake encryption.
- Compress/Unlock use raster rebuilding and may remove selectable text.
- PDF-to-Word is a simple text-layer extraction rather than full DOCX reconstruction.
- Sign PDF uses a typed signature overlay in this baseline.
