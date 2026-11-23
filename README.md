# antariksh-client-brief-v2

Antariksh Design Studio – client design brief (English + Gujarati).

Live link: https://hiren7784.github.io/antariksh-client-brief-v2/

- `index.html` – the whole form (styles and script inside). GitHub Pages only opens a file named exactly `index.html` at the main link, so keep this name when uploading a new version.
- `js/pdf-lib.min.js` – pdf-lib 1.17.1 (MIT, licence in `js/pdf-lib-LICENSE.txt`). Loaded only on the last two steps, to make the brief PDF. Upload the `js` folder together with `index.html`.
- `.nojekyll` – tells GitHub Pages to serve the files as they are.

## How the last page sends the brief

When the client presses Next into the last page, the form packs everything into one ZIP:

```
Antariksh-Brief-<Name>/
  Antariksh-Brief-<Name>.pdf    brief with photo previews and a list of every file
  Antariksh-Brief-<Name>.json   the same answers as data (import into team.html)
  files/01-site-photo.jpg       every uploaded file exactly as uploaded,
  files/02-plan.dwg             numbered as in the PDF list
```

- **Send ZIP on WhatsApp** (main button): the ZIP downloads and the Antariksh chat (+91 76210 03444) opens with the brief typed in. The client taps the paperclip → Document, picks the ZIP and presses Send. Browsers do not let a website hand a ZIP straight to WhatsApp on Android or computers, so this attach step is needed. On iPhone the share menu is tried first.
- **Share PDF & photos** (phones only, one tap): the share menu opens with the PDF plus photos/PDFs as separate files. DWG, Word and other types travel inside that PDF as attachments (open in Adobe Acrobat Reader → paperclip panel).
- **Download ZIP / Download PDF / Send as text message only** are small links under the buttons.

Limits: up to 20 files, 25 MB each, 40 MB in total.

Answers and files are kept only in the client's browser (files in IndexedDB) until they send them; nothing is stored on a server.
