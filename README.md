# Crushers Sports: public site (client side only)

Static HTML/CSS: Home and Trainers pages. No login yet. Parent login will be added later (the earlier `crushers-sports-site` package has a Supabase-based version ready).

## Preview locally
    cd crushers-sports-public
    python3 -m http.server 8000     # open http://localhost:8000

## Publish on GitHub Pages
1. Create a GitHub repo and push these files (`git init`, `git add .`, `git commit`, `git push`).
2. Settings > Pages > Deploy from branch `main`, folder `/ (root)`. Custom domain is set by the `CNAME` file (crusherssports.org); tick Enforce HTTPS.
3. At your registrar, add four A records for the apex domain: 185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153, plus a CNAME `www` -> YOUR-GITHUB-USERNAME.github.io (confirm IPs in GitHub's docs). Forward crusherssports.com to the .org.

## Editing
- Trainer cards: `trainers.html` (placeholders now)
- Colors: top of `css/style.css`
- Logo: `img/logo.jpg`
