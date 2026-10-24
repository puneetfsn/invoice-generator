# Invoice Studio

A free, browser-based invoice generator for freelancers and small businesses. Like [SnapFrame](https://github.com/puneetfsn/snapframe), it is a static web app: no account, build step or backend required.

**Live app:** https://puneetfsn.github.io/invoice-generator/

## What it does

- Add business and client details, a logo, invoice dates and currency
- Add or remove line items with automatically calculated totals, discount and tax
- Optionally add a diagonal business-name watermark (or custom text), with horizontal and vertical alignment controls
- Choose a custom invoice background color
- Preview an A4-style invoice as you type
- Download a PDF or use the browser’s Print → Save as PDF option
- Automatically save the current invoice in your browser’s localStorage

## Run locally

Open `index.html` in a browser, or run `python3 -m http.server 8000` from this folder and visit http://localhost:8000/. The previous `invoice-generator.html` URL redirects to the app.

PDF export loads [html2pdf.js](https://github.com/eKoopmans/html2pdf.js) from a CDN, so an internet connection is required for the PDF button. If the library cannot load, use Print → Save as PDF. Editing and preview work offline.

Watermarks are visual branding only and do not verify a business. For colored backgrounds when using Print → Save as PDF, turn on **Background graphics** in the browser print settings.

Your invoice and uploaded logo stay in the current browser's localStorage. Clearing site data or switching browsers will remove them; there is no server-side backup.

## Hosting

The app is published with GitHub Pages from `main` at `/ (root)`. Changes appear on the live site after they are merged to `main` and Pages finishes rebuilding.

## Search visibility

The homepage has a descriptive title, visible introduction, canonical URL, social sharing metadata and WebApplication structured data. The sitemap is available at https://puneetfsn.github.io/invoice-generator/sitemap.xml.

To request indexing, add `https://puneetfsn.github.io/invoice-generator/` as a **URL-prefix property** in [Google Search Console](https://search.google.com/search-console/), complete ownership verification using the method Google provides, submit the sitemap URL, and request indexing for the homepage. Verification requires your own Search Console code or file; it is not included in this repository. Indexing and rankings are not guaranteed.
