# AviNotes Studio v2
Upload these files to the root of your existing `avinotes` GitHub repository, replacing the previous versions.

## New in v2
- Pencil-only mode (ignores touch drawing by default)
- Optional finger + Pencil mode
- Ball pen, fountain-style pen, brush, pencil-style ink, highlighter and eraser
- Stroke smoothing control
- Optional pressure-based width where browser stylus events provide pressure
- Ruled, grid, dotted and blank paper
- Undo/redo, clear page, local autosave, search and JSON backup
- Keeps the same IndexedDB database name and note store, so existing notes should remain available

## Important iPad limitation
This is a web app. It can ignore touch drawing while in Pencil-only mode, but cannot guarantee native iPadOS-level palm rejection. Pressure data and stylus identification depend on the iPad, stylus, Safari and browser event support. This app does not claim to reproduce native Goodnotes/CollaNote ink rendering.

## Update GitHub
Replace `index.html`, `manifest.webmanifest`, and `sw.js` in the existing repository root. Commit the changes. Then reload the website on iPad. If the old version persists, close the installed web app fully and reopen it; the service worker cache version has been bumped.
