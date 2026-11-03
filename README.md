# Vanderbilt Energy Transition Society (ETS)

Simple static website for Vanderbilt’s Energy Transition Society. No build tools — edit HTML/CSS and push.

**Live site (once Pages is on):** `https://rhettadam.github.io/vandy-ets-website/`

## Enable GitHub Pages

1. Go to the repo on GitHub → **Settings** → **Pages**
2. Under **Build and deployment**, set **Source** to **Deploy from a branch**
3. Branch: `main` / folder: `/ (root)` → **Save**
4. Wait a minute, then open the Pages URL

## Edit content

Almost everything lives in `index.html`. Look for the section comments:

| Section | What to change |
|---|---|
| Hero | Headline, short blurb, button links |
| About | Org description |
| Get Involved | Steps / meeting cadence |
| What We've Done | Timeline items (add/remove `<li>`) |
| Contact | Email and social links |

Colors and fonts are CSS variables at the top of `styles.css` (`:root`).

Logo: `assets/logo.jpg` (nav, hero, and favicon).  
Hero photo: replace `assets/hero.webp` (keep the same filename, or update the `<img src>`).

## Local preview

Open `index.html` in a browser, or from this folder:

```bash
# Python
python -m http.server 8000

# Node
npx serve .
```

Then visit `http://localhost:8000`.

## Stack

- Plain HTML + CSS + a tiny bit of JS (year + mobile nav)
- Hosted free on [GitHub Pages](https://pages.github.com/)
