# Helen's Home Care — Website

Astro + Tailwind CSS marketing site for Helen's Home Care LLC.

## Local development
```bash
npm install
npm run dev        # http://localhost:4321
```

## Build & serve (what Railway runs)
```bash
npm run build      # outputs static site to dist/
npm start          # serves dist/ on $PORT
```

## Deploy to Railway
1. Push this folder to a GitHub repo.
2. railway.app → New Project → Deploy from GitHub repo → select the repo.
3. Railway auto-detects Node, runs `npm run build`, then `npm start`.
4. Settings → Networking → Generate Domain.
5. (Custom domain) Add domain in Railway, then create the CNAME it shows at your DNS provider.

## Before launch — replace placeholders
- Phone number `(214) 555-0123` (appears in header, footer, and all pages)
- Email `care@helenshomecare.com`
- HHSC license number `#000000` in the footer (src/layouts/Base.astro)
- Contact form: create a free form at formspree.io and replace `YOUR_FORM_ID` in src/pages/contact.astro
