# Invoice Studio

A lightweight, single-file invoice generator for freelancers and small businesses. Create invoices, see an instant A4-style preview, and download a PDF. Your invoice is saved automatically in your browser's localStorage; no account or backend is required.

## Use

Open `invoice-generator.html` in a browser (or serve it with any static HTTP server). Fill in your business and client details, add line items, and click **Download PDF**. Use **New invoice** to clear the saved invoice after confirmation.

PDF export loads [html2pdf.js](https://github.com/eKoopmans/html2pdf.js) from a CDN, so an internet connection is required for the PDF button. If the library cannot load, use your browser's Print dialog to save as PDF instead. Other editing and preview features work offline.

Data and logos stay in the current browser's localStorage. Clearing site data or switching browsers will remove them. There is no server-side backup.
