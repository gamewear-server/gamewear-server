# Gamewear Warehouse server address

`server.json` stores the current Gamewear Warehouse tunnel URL. The Android
application and the web launcher read this file so workers do not need to know
when the tunnel address changes.

The web launcher is `index.html`. After GitHub Pages is enabled for the `main`
branch, workers can keep one permanent bookmark:

`https://gamewear-server.github.io/gamewear-server/`

The page always fetches a fresh copy of `server.json`, validates the returned
HTTP/HTTPS URL, and redirects the browser to the normal warehouse sign-in page.
