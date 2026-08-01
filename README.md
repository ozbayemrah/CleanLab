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
2. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**.
3. Pick the `main` branch and `/ (root)` folder, then save.
4. GitHub gives you a URL like `https://yourname.github.io/cleanlab-site/` within a minute or two.

## What's in `assets/`

- `CleanLab.svg`, your real logo, used in the nav and footer.
- `CL-mascot.svg`, your real mascot illustration, used in the hero and "how it's made" section.

Swap either file for an updated version any time. The filenames are referenced directly in `index.html`, so a same-name replacement needs no code changes.

## What's on the page

- Sticky nav with the real logo
- Scrolling ticker strip with brand claims (vegan, garage-made, biker-approved)
- Hero with the mascot and the "mad science, clean conscience" tagline
- Three product cards for Flower Fart, BubbleGum, CleanDisco with dummy prices and "notify me" buttons
- "How it's made" story section pairing the mascot with the vegan/eco claims
- A three-step process strip (mix, bottle, ride)
- A SoxyBobby socks teaser block
- An email signup section, currently just swaps the button text to a confirmation message. Wire the form up to Mailchimp, Buttondown, a Google Form, or similar before a real launch
- Footer with logo, nav links, and placeholder social links

Everything is one HTML file with inline CSS/JS, so it's easy to hand-edit directly. No build tools needed, matching the zero-cost setup.

## Easy next tweaks

- Real prices once you've set them (search for "14.90" in index.html)
- Real Instagram/TikTok links in the footer (search for href="#")
- Swap the placeholder product swatch colors/bottle shapes for real product photography once you have it
