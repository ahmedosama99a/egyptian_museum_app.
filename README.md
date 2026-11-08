# Egyptian Museum AI Website

React + Vite website for hieroglyph scanning, multilingual meanings, audio, and an educational symbol dictionary.

## Run locally

```bash
npm install
npm run dev
```

Open the local URL shown by Vite, normally `http://localhost:5173`.

## Publish with GitHub Pages

1. Create a new GitHub repository.
2. Upload all files and folders from this project root. Do not upload the outer ZIP file.
3. Use the `main` branch.
4. Open repository **Settings > Pages**.
5. Under **Build and deployment**, select **GitHub Actions**.
6. Open the **Actions** tab and wait for `Deploy website to GitHub Pages` to finish.
7. The website URL will appear in the deployment summary and in **Settings > Pages**.

The included workflow builds the Vite app and deploys the `dist` folder automatically after every push to `main`.

## Important limitation

GitHub Pages hosts static frontend files only. It cannot run `backend/api.py`, PyTorch, or FastAPI. The frontend therefore uses its demo fallback when the API is unavailable.

For real AI recognition, deploy the `backend` folder separately to a Python hosting service such as Render, Railway, or Azure App Service, then replace `http://localhost:8000/predict` in `src/App.jsx` with the public HTTPS backend URL.

## Camera

Browser camera access works on HTTPS. GitHub Pages provides HTTPS, so users can grant camera permission after the site is deployed.
