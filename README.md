# Workshop 3 — Compare & Contrast Essay (Word download repair)

Fixed a JavaScript variable shadowing bug: the DOCX export previously declared `let document` inside the download function and then attempted `document.createElement('a')`, treating the Word XML string as the browser document. It now uses `documentXml` so the browser download link can be created.

Upload all four files together to the same GitHub Pages folder, replacing the originals. Hard refresh (Ctrl+Shift+R). Existing browser progress uses the same storage key and should remain available on the same browser, but students should download a JSON progress backup before updating.

The Word export can be used on incomplete drafts; when the full essay is empty, it assembles the existing paragraph drafts. The JSZip library is included locally.
