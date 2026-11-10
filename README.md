# Multiplayer Board: tldraw sync proof of concept

A shared whiteboard. Everyone who opens the same `?room=` link draws on the same canvas live, with cursors, names, and presence.

- **Live:** https://mayawalsh19-art.github.io/multiplayer-poc/
- **Stack:** Vite + React + `tldraw` + `@tldraw/sync` (`useSyncDemo`, which uses tldraw's hosted demo sync server)
- **Deploy:** push to `main` and GitHub Actions builds it and publishes to Pages

## Run locally
    npm install
    npm run dev

## Notes
- The demo sync server is for prototyping: rooms are public to anyone with the ID and get wiped after about a day.
- For something real, swap `useSyncDemo` for `useSync` pointed at your own server (tldraw's `sync-cloudflare` template).
