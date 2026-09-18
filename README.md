# PDF Tools — GitHub-ready browser PDF toolkit

A static, browser-first PDF utilities site designed for GitHub Pages, Netlify or Vercel.

## UI/UX highlights
- Tailwind CSS CDN + custom responsive design system
- Blue/teal visual theme with light/dark mode
- Font Awesome icons
- Mobile/tablet/desktop responsive layout
- Animated loading screen, cards and progress states
- Drag & drop file selection
- Smart PDF page preview with page selection and zoom
- Live HTML preview for HTML-to-PDF
- Client-side processing with no required upload backend

## Deploy to GitHub Pages
1. Create a new repository.
2. Upload the contents of this folder (not the ZIP itself).
3. Commit to `main`.
4. GitHub → Settings → Pages → Source: GitHub Actions.
5. The included workflow deploys the site automatically.

## Custom domain
Rename `CNAME.example` to `CNAME`, then put `pdf.bishnulamsal.com.np` inside it and configure your DNS for GitHub Pages.

## Important limitations
- Protect PDF does not fake encryption.
- Compress/Unlock use raster rebuilding and may lose selectable text.
- PDF-to-Word exports extracted text to a Word-compatible `.doc`; complex layout/OCR is not reconstructed.
- HTML-to-PDF is a browser render/export workflow.

## CDN dependencies
Font Awesome 7.3.1, Tailwind CSS CDN, pdf-lib 1.17.1, PDF.js 4.10.38, JSZip 3.10.2, FileSaver.js 2.0.5, html2canvas 1.4.1 and jsPDF 4.2.1.
