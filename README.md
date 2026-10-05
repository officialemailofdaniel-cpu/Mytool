# FileForge — Production PDF Tool Set

This version follows one rule: **a feature is not shown unless it is implemented.**

## Implemented browser-side tools
- Merge PDF
- Split PDF
- Extract PDF pages
- Delete PDF pages
- Reduce PDF size (real rendered/JPEG rebuild; text/searchability can be lost)
- JPG/PNG/WebP to PDF
- PDF to JPG/PNG
- Rotate PDF
- Text watermark
- Page numbers
- Crop PDF
- PDF to Text (selectable text)
- OCR to Text for scanned PDFs

No fake Word/Excel/PowerPoint/security/AI buttons are included.

## Libraries
- PDF-LIB
- PDF.js
- Tesseract.js (loaded only when OCR is used)
- JSZip (loaded only when PDF-to-images is used)

## Deployment
Upload the files to GitHub and connect the repository to Cloudflare Pages as a static site.

Important: browser-side processing is convenient and private, but very large PDFs can use significant RAM. For a production-scale service, add a Cloudflare Worker/server processing tier later.
