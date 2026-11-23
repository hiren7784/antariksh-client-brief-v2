# antariksh-client-brief-v2

Antariksh Design Studio – client design brief (English + Gujarati).

Live link: https://hiren7784.github.io/antariksh-client-brief-v2/

- `index.html` – the whole form (styles and script inside). GitHub Pages only opens a file named exactly `index.html` at the main link, so keep this name when uploading a new version.
- `js/pdf-lib.min.js` – pdf-lib 1.17.1 (MIT, licence in `js/pdf-lib-LICENSE.txt`). Loaded only on the last two steps, to make the brief PDF. Upload the `js` folder together with `index.html`.
- `.nojekyll` – tells GitHub Pages to serve the files as they are.

## How "Share via WhatsApp" works

On the last step the form makes a PDF of the answers, with previews of the client's photos and a list of every reference file.

- **Phone (and Windows/Mac browsers that have a share menu):** the share menu opens with the PDF plus the photos and PDFs as separate files. The client picks WhatsApp → Antariksh Design Studio (+91 76210 03444) → Send.
- **DWG, DXF, SketchUp, Revit, Word, Excel and other files:** browsers are not allowed to hand these to WhatsApp, so they travel **inside the PDF** as attachments. Open the PDF in Adobe Acrobat Reader; the Attachments (paperclip) panel opens by itself and lists them.
- **Browsers without a share menu (e.g. Firefox):** the PDF downloads with every file inside it, and WhatsApp opens the Antariksh chat; the client attaches the PDF.
- **Send as text message only** opens the Antariksh chat with all answers typed in (no files).

Limits: up to 20 files, 25 MB each, 40 MB in total. One share carries the PDF plus at most 9 separate files (the browser refuses more than 10); any extra files go inside the PDF.

Answers and files are kept only in the client's browser (files in IndexedDB) until they share them; nothing is stored on a server.
