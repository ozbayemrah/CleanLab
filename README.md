# CleanLab, demo site

A single-page demo built for GitHub Pages. No build step, no dependencies, just `index.html` plus the `assets/` folder.

## Run it locally

Open `index.html` directly in a browser, or serve the folder:

```
python3 -m http.server 8000
```

then visit `http://localhost:8000`.

## Put it on GitHub Pages

1. Create a new repo (e.g. `cleanlab-site`) and push these files to it (`index.html`, `assets/`, this `README.md`).
2. In the repo: **Settings -> Pages -> Build and deployment -> Source: Deploy from a branch**.
3. Pick the `main` branch and `/ (root)` folder, then save.
4. GitHub gives you a URL like `https://yourname.github.io/cleanlab-site/` within a minute or two.

## What's in `assets/`

- `CleanLab.svg`, your real logo, used in the nav and footer.
- `CL-mascot.svg`, your real mascot illustration, used in the hero and "how it's made" section.

Swap either file for an updated version any time. The filenames are referenced directly in `index.html`, so a same-name replacement needs no code changes.

## What's on the page

- Sticky nav with the real logo and a mobile hamburger menu
- Scrolling ticker strip with brand claims (vegan, water/formula ratio, hand made, scratch safe, hard water compatible)
- Hero with your real mascot art and the "mad science, clean conscience" line
- **The lab shop**: a full product catalog of 8 base products across 22 scent/colour variants (Ready Cleaner, Ready Cleaner + Concentrate Refill, Refill Drivetrain Cleaner, Lube, Shine Protection, SoxyBobby socks, Cap, Care Kit), each in the Flower Fart, BubbleGum or CleanDisco scent lines where it applies. Filterable by availability, product type, price range and colour, sortable by price, name or newest, styled after the Muc-Off collection page layout but kept in CleanLab's own visual style.
- **What's New** strip showing the newest badged items
- Click any product tile to open a full detail popup with tabs for Description, Product info, Features, How to, Protect the world, FAQ and Reviews. All content is placeholder, edit the `BASE_PRODUCTS` and `VARIANTS` objects near the bottom of `index.html` to change it.
- **Trend topics** section (New Releases, Upcoming Products, Our Community, Instagram)
- A floating **Lab Assistant** chat widget bottom right. This is a scripted keyword-matching demo, not a real AI, it's clearly labeled as such in the UI. Edit the `RULES` array in the script to change its answers, or replace it with a real chatbot/LLM integration later.
- Email signup section, UI only, not wired to anything
- Footer with Shop, Help, Lab and Legal columns, social links, and an imprint/privacy/terms placeholder row (Austria requires an Impressum once this goes live, add real legal pages before launch)

Everything is one HTML file with inline CSS/JS, so it's easy to hand-edit directly. No build tools needed, matching the zero-cost setup.

## Easy next tweaks

- Real prices once you've set them (search for the base prices in the `VARIANTS` array in `index.html`)
- Real Instagram/TikTok/Facebook links in the footer and trend topics section (search for `href="#"`)
- Real legal pages (Imprint, Privacy Policy, Terms) before this goes live, currently placeholders
- Swap the placeholder colour swatches for real product photography once you have it
- Connect the email signup form and the Lab Assistant to real services when you're ready to launch
