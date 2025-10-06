# Mappa Vico Equense — Leaflet + Classifica

Sito statico pronto per **GitHub Pages**: mappa con pin (Leaflet) e classifica per squadre basata su `foundBy` in `pins.json`.

## Come pubblicare

1. Crea un repository su GitHub (pubblico), es. `mappa-vico`.
2. Carica **tutti i file** di questa cartella (index.html, pins.json, .nojekyll, README.md).
3. Vai su **Settings → Pages → Build and deployment → Deploy from a branch**, scegli **`main`** e cartella **root** `/`.
4. Attendi l'URL pubblico della pagina.

## Come aggiornare i pin e la classifica

- Apri `pins.json` su GitHub, modifica il campo `foundBy` del pin trovato (es. "rossi", "blu", "verdi", "gialli").
- Esegui **Commit changes**. La pagina si aggiornerà automaticamente al refresh.
- Per aggiungere un nuovo pin, inserisci un nuovo oggetto con `id`, `lat`, `lng`, `title`, `desc`, `foundBy`.

## Suggerimenti

- Per ottenere coordinate precise, apri la pagina, premi **F12 → Console**, clicca sulla mappa: vedrai `Nuovo pin: {lat: ..., lng: ...}`.
- Personalizza i colori squadra in `TEAM_COLORS` dentro `index.html`.
- Il parametro `?ts=Date.now()` nel `fetch` evita la cache di GitHub Pages.

Buon divertimento!
