# LearnWell Academy — Website

A premium, editorial-style single-page website for **LearnWell Academy**, a UK-based online STEM tuition centre.

## Files in this repo

- **`index.html`** — the entire website (HTML, CSS and JavaScript embedded in one file).
- **`netlify.toml`** — Netlify configuration with sensible security headers and caching.
- **`README.md`** — this file.

That's it. No build step, no dependencies, no npm. Open `index.html` in any browser to preview.

---

## How to publish (free, in about 5 minutes)

### Option 1 — Drag-and-drop to Netlify (easiest)

1. Go to <https://app.netlify.com/drop>
2. Drag the **entire `learnwell` folder** onto the page.
3. Netlify gives you a URL like `https://elegant-curie-12345.netlify.app` — your site is live.
4. To rename: in Netlify, go to **Site settings → Change site name** and pick something like `learnwell-academy`.

### Option 2 — GitHub + Netlify (best for editing later)

1. Create a new repo on GitHub (e.g. `learnwell-academy-site`).
2. Upload these files to the repo (you can drag-and-drop on the GitHub site).
3. On Netlify, click **Add new site → Import from Git → GitHub** and pick the repo.
4. Click **Deploy** — Netlify will auto-deploy on every push to `main`.

After this is set up, **any change you push to GitHub automatically updates the live site** within ~30 seconds. Perfect for editing copy or adding sections later.

---

## How to edit the content

Everything lives in `index.html`. Use Notepad, VS Code, or any text editor.

Common edits, with `Ctrl+F` search terms to find them:

| What you want to change | Search for |
|---|---|
| Email address | `learnwellaca@gmail.com` |
| Subjects offered | `<!-- ============= SUBJECTS` |
| Levels grid | `<!-- ============= SUBJECTS` (scroll to "levels-table") |
| About section text | `<!-- ============= ABOUT` |
| Weekly exam feature | `<!-- ============= FEATURE` |
| Tutors quote | `<!-- ============= TUTORS` |
| How-it-works steps | `<!-- ============= HOW IT WORKS` |
| Stats numbers | `<!-- ============= TRUST` |
| Footer copy | `<footer>` |

### Changing colours

All colours are defined as CSS variables at the very top of the `<style>` block. Edit these and everything updates:

```css
--navy:        #0A2342;   /* primary deep navy */
--gold:        #C9A961;   /* warm gold accent */
--teal:        #2E6171;   /* secondary teal */
--ivory:       #F7F4ED;   /* page background */
```

---

## Custom domain (optional, ~£8/year)

Once you're happy with the site:

1. Buy a domain — try `learnwellacademy.co.uk`, `learnwell.academy`, or `learnwelltuition.co.uk` from Namecheap, GoDaddy, or 123-reg.
2. In Netlify: **Domain management → Add custom domain**, then follow the DNS instructions.
3. Netlify provides free HTTPS automatically.

---

## What's in the design

- **Fonts**: Fraunces (display serif) + Outfit (body sans) + Cormorant Garamond (accents) — loaded from Google Fonts.
- **Palette**: Premium navy + warm gold + ivory — consistent with the LearnWell mock papers.
- **Animations**: Subtle scroll-reveal effects, a scrolling marquee of subjects/boards, floating hero badges, hover transitions on cards.
- **Responsive**: Tested layouts for desktop (1280px+), tablet (1024px), and mobile (640px down to 320px).
- **Accessibility**: Semantic HTML, sufficient colour contrast, keyboard-navigable, mobile menu.
- **Performance**: Single HTML file, no images that aren't decorative SVGs, no third-party scripts beyond Google Fonts. Loads in well under a second.

---

## Sections in order

1. Sticky navigation (transparent → solid on scroll)
2. Hero with animated decorative card and floating badges
3. Subjects/boards marquee
4. About — philosophy + four pillars
5. Subjects — four cards + complete levels table
6. Exam boards — AQA, Edexcel, OCR
7. How it works — 4-step process
8. Weekly exams feature — with sample progress card
9. Tutors — credentials with pull-quote
10. Class formats — small group + Teams delivery
11. Stats / trust band
12. CTA — email signup that opens a prefilled `mailto:` link
13. Footer

---

## Need to update?

The site is plain HTML so AI assistants (including me, Claude) can edit anything easily. Just say what you want changed and paste the relevant section.

— Built for LearnWell Academy · *Inspiring Excellence*
