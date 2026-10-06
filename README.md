# Tender Document Package Builder (AI DevFest 2026)

- **Name:** <YOUR NAME>
- **Registration number:** <YOUR REG NO>
- **Live link (HTTPS):** <ADD AFTER DEPLOY>

## How to run
```
npm install
npm run dev      # local development
npm run build    # output in dist/ (deploy this folder)
```
Deploy settings (Vercel / Netlify / Cloudflare Pages): build command `npm run build`, output directory `dist`.

## Main features done
- Load requirements.json (sorted by order), tender details shown
- Upload many PDFs, name and page count, non-PDF rejected, remove files
- Match files to requirements (1 file : 1 requirement), change or clear any time
- Expiry date input, live status (Missing, Expiry date needed, Expired, Not provided, OK)
- Duplicate detection by SHA-256 of file content; duplicate copies cannot be matched to different documents
- Generate button disabled with reasons; cover page, ordered documents, footer `<tender_id> | Page X of Y` on every page (in an added white strip, content is never covered)
- Download `<tender_id>_Package.pdf`
- Full Bangla / English switch

## Bonus features done
- Checklist export (CSV, UTF-8 with BOM)
- Damaged and password-protected PDFs show a message instead of crashing

## Known problems
- Cover page is English only (Bangla not drawn on the PDF)
- No index page, seal or save/reopen
- Annotations and form fields inside source PDFs are flattened to page content

## AI tools used
<FILL IN>

## Most useful prompt
<PASTE YOUR BEST PROMPT>
