# AviNotes Studio v3
Upload these files to the root of the existing `avinotes` GitHub repository, replacing previous versions.

## Improvements
- Active stylus mode: only Pointer Events reported as `pen` are accepted.
- Universal/capacitive mode: accepts touch-like stylus events with optional contact-size filtering.
- Finger writing mode.
- Contact guard and adjustable maximum touch contact size.
- Coalesced pointer-event samples for smoother strokes.
- Adjustable smoothing and pen thickness.
- Pressure-based width only when the browser reports a pen event and pressure is enabled.
- Ball, fountain-style, brush, pencil-style, highlighter and eraser tools.
- Ruled/grid/dotted/blank pages, undo/redo, local autosave, JSON backup.
- Uses the same IndexedDB database and object store as v1/v2.

## Stylus limitations
Many passive capacitive styluses are reported by iPad Safari as `touch`, just like a finger. Choose Universal/capacitive mode for those. Contact-size filtering is heuristic and varies by browser/device; it cannot guarantee palm rejection. A true active stylus with iPadOS palm rejection and pen input support is recommended for reliable writing.

## Deploy update
Replace `index.html`, `manifest.webmanifest`, and `sw.js` in the existing GitHub repository root. Commit changes. Reload the web app. If the old version remains, fully close the installed web app and reopen it, or reload Safari after a short wait.
