# AviNotes v1
A free, installable-web-app starter for iPad.

## Included
- Typed notes
- Finger/Apple Pencil drawing canvas (browser pointer events)
- Pen colour and size, eraser, undo, clear
- Local offline-capable storage using IndexedDB
- Search, delete, JSON export/import backup
- PWA manifest and service worker

## Run
For a quick local preview, open `index.html` in a browser. For installation/offline PWA support, host the folder on an HTTPS static host (for example GitHub Pages). On iPad Safari: Share -> Add to Home Screen.

## Important storage note
This first version saves on the current iPad/browser only. Export a JSON backup regularly. Cloud sync is intentionally not enabled yet: it needs a cloud project and sign-in/security setup. The next milestone is adding Supabase Auth + database + private per-user storage, with local-first sync. Never put a Supabase service-role key in frontend code; only use the anon/publishable key with Row Level Security policies.

## iPad notes
- Best drawing experience is with Apple Pencil, but finger input also works.
- This is a web app, not a native App Store app.
- Test pencil input and page behaviour on your iPad before relying on it for important notes.
