# AJRCrypto

Two-page crypto dashboard:

- `index.html` — Live prices + news + chart (AJRCrypto brand)
- `what-if.html` — What-If Analysis with presets and 6/12/18-month projections

## Run locally
Just open `index.html` in your browser, or serve the folder:
```bash
python -m http.server 8080
```

## Deploy to Vercel (no build)
1. Create a new GitHub repo (e.g., `ajrcrypto`).
2. Push these files:
   ```bash
   git init
   git add .
   git commit -m "init: AJRCrypto"
   git branch -M main
   git remote add origin https://github.com/<your-username>/ajrcrypto.git
   git push -u origin main
   ```
3. In Vercel: **New Project → Add Git Repository → Import**
   - Framework: **Other**
   - Build Command: *(leave blank)*
   - Output Directory: `/`
4. Deploy. Your **source repository URL** is the GitHub link above.

_(Optional)_ Add a CryptoPanic token in the UI on the home page to fetch headlines.
