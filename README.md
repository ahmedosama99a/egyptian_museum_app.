# Hieroglyph Quest Pro - Fixed

Fixes the startup freeze caused by the information modal appearing even while it had the HTML `hidden` attribute. The modal now remains closed until a symbol card is selected. Escape, background click, and the close button close it correctly. Audio includes browser support checks and a slower Arabic speech rate.

## Deploy to GitHub Pages
Replace the old repository files with:
- `index.html`
- `style.css`
- `app.js`
- `README.md`

Commit the changes and hard-refresh the published page with `Ctrl + F5`.

For reliable testing, use the GitHub Pages HTTPS URL. Do not test by double-clicking `index.html` with a `file:///` address because browser security and speech behavior can differ.
