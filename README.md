# landing-page

Static landing page using the `free-lite` template. The site is published via GitHub Pages using the workflow in [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml).

## Deployment

1. Enable **GitHub Pages** for the repository and choose **GitHub Actions** as the source (Settings → Pages).
2. Push to the `main` branch or trigger the **Deploy free-lite static site to GitHub Pages** workflow manually from the **Actions** tab.
3. The workflow uploads everything under `free-lite/` as the published site. If you add new assets, make sure they live in that folder so they are included.
4. After the workflow completes, the page URL is available in the run summary under the `deployment` step output.

## Local preview

Open `free-lite/index.html` directly in a browser, or serve it locally for a closer match to GitHub Pages:

```bash
cd free-lite
python -m http.server 8000
```

Then browse to http://localhost:8000.
