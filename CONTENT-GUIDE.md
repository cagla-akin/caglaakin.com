# How to edit caglaakin.com

Two ways to make changes:

**In the browser:** open this repo on github.com → click the file → ✏️ pencil icon → edit → **Commit changes**. Live in ~1 minute.

**Locally:** edit the files in `~/Desktop/personal-website/`, then in Terminal:

```
cd ~/Desktop/personal-website
git add -A && git commit -m "describe your change" && git push
```

## Where everything lives

All text content is in **`index.html`**. Search (⌘F) for a phrase you can see on the site to jump to it. Landmarks:

| To change… | Search for… |
|---|---|
| Headline roles ("Data Science & AI · …") | `hero-roles` |
| "Hello world" intro | `Hello world` |
| Scrolling ticker words | `ticker-track` (edit BOTH copies — they must be identical) |
| About text | `Finance Manager` |
| Facts table (Based in / Focus / Education / Tools) | `about-facts` |
| Expertise cards | `expertise-grid` |
| Spotify project blurb + links | `Featured project` |
| Music / Sunrise Fiancée section | `After dark` |
| Contact email | `hello@caglaakin.com` |
| Social links (sidebar + contact) | `sidebar-social` and `contact-links` — replace the `#` in `href="#"` with your URL |

## Photos

Photos live in `images/`:
- `sidebar.jpg` — small square photo, left panel
- `about.jpg` — portrait in the About section
- `music.jpg` — DJ photo in the Music section

To swap one: replace the file with a new image **using the same filename** (on GitHub: open `images/` → Add file → Upload files). Keep photos under ~500KB for fast loading.

## Resume

`Cagla-Akin-Resume.pdf` is what the "Download my resume" button serves. Replace the file (same name) to update it. Remember it's public — no phone number or personal email.

## Colors, fonts, layout

All in `styles.css`. The palette is defined at the top in `:root` — e.g. `--accent` is the terracotta orange. Changing layout/CSS by hand is riskier than text edits; consider asking Claude for these.

## Things to be careful about

- Don't delete the `CNAME` file — it connects the caglaakin.com domain.
- In HTML, `&amp;` renders as `&` — keep the `&amp;` form when editing text.
- If you break something and the site looks wrong: on github.com open the file → **History** → open the last good version → copy it back (or ask Claude to revert).
