# Krushnam Thoria — Creative Developer Portfolio

React + Tailwind CSS + Vite portfolio built around the details and 13 public App Store links from `Krushnam_Thoria.pdf`.

## Included
- Animated creative hero, selected work, 13-app gallery with AI/iOS filters, skills, experience, contact.
- Featured BetterSwing, Astro11, DragonAI, and AI Calendar Agent.
- **Real original App Store artwork/screenshots**: the site requests these from Apple's official public iTunes lookup endpoint in the visitor's browser. It displays official images only when API data is available; otherwise, it shows a placeholder. No AI-generated product screenshots.
- CV download in `public/Krushnam_Thoria_CV.pdf`.
- GitHub Pages deployment workflow.

## Quick start

```bash
npm install
npm run dev
```

Open the local URL printed by Vite. To check a production build:

```bash
npm run build
npm run preview
```

## Profile links configured

- LinkedIn: https://www.linkedin.com/in/krushnam-thoria-%EF%A3%BF-42300658/
- GitHub: https://github.com/krushnamios
- Email: krushnamios@gmail.com
- Resume: `public/Krushnam_Thoria_CV.pdf` (public download; includes a phone number).

Before publishing, review project descriptions for confidential client details. Official App Store artwork loads from Apple's API where available, with graceful placeholders otherwise.

## Publish to your GitHub Pages URL

**Target:** `https://krushnamios.github.io/` (not live until you publish).

1. Sign into GitHub as `krushnamios` and create a new **public** repository named **`krushnamios.github.io`**. Do not initialize it with a README.
2. Extract this ZIP, open a terminal inside the `krushnam-creative-portfolio` folder, then run:

```bash
git init
git add .
git commit -m "Launch creative developer portfolio"
git branch -M main
git remote add origin https://github.com/krushnamios/krushnamios.github.io.git
git push -u origin main
```

3. In the repository, go to **Settings → Pages → Build and deployment → Source: GitHub Actions**.
4. Open **Actions** to confirm that the included deploy workflow succeeds. The public site will appear at `https://krushnamios.github.io/` once GitHub completes deployment. Repository settings/policies may affect availability.

A GitHub token or password should never be shared in chat. If a login prompt appears, authenticate securely with GitHub's own login flow.

## Apple lookup implementation

`src/main.jsx` uses calls shaped like:

`https://itunes.apple.com/lookup?id=6794278013&country=us&entity=software`

The app ID and territory originate from the CV. Apple may change or limit the response. Apple provides catalog metadata; this project does not guarantee that every screenshot is returned in every territory.

## Privacy

The site displays the public professional email from the resume, but it intentionally does **not** print the phone number. The original PDF resume contains the phone number and is downloadable. Remove it from the PDF if you do not wish to make the number public.
