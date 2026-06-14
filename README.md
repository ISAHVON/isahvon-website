# ISAHVON Website

A responsive, premium one-page website for **ISAHVON**, a Karlstad-based DJ brand available across Sweden and worldwide.

## What is included

- `index.html` — semantic HTML5 landing page
- `styles.css` — responsive dark luxury UI with animations and media placeholders
- `script.js` — Swedish/English language toggle, mobile menu, reveal animations and email inquiry handling
- No build tools required
- GitHub Pages friendly

## Contact details already included

- Email: `Isahvon@outlook.com`
- Phone: `079 349 59 29`
- Phone link: `tel:+46793495929`
- Instagram: `https://www.instagram.com/ISAHVON/`

## How to run locally

Open `index.html` directly in your browser.

For a better local preview, you can use VS Code with the **Live Server** extension.

## How to publish on GitHub Pages

1. Create a new GitHub repository, for example `isahvon-website`.
2. Upload these files to the repository root.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/root`
5. Save.

GitHub will give you a live URL after deployment.

## How to replace placeholders with real media

### Hero background

In `styles.css`, look for `.hero-bg`. You can add a real image like this:

```css
.hero-bg {
  background:
    linear-gradient(90deg, rgba(9, 9, 9, 0.95), rgba(9, 9, 9, 0.67), rgba(9, 9, 9, 0.86)),
    url("assets/hero.jpg") center / cover no-repeat;
}
```

Create an `assets` folder and add your image as `hero.jpg`.

### Audio / video embeds

Replace the placeholder blocks inside the `#media` section in `index.html` with SoundCloud, Spotify, YouTube, Vimeo or Instagram embeds.

Use `loading="lazy"` on iframes for performance.

Example:

```html
<iframe
  loading="lazy"
  title="ISAHVON mix"
  src="YOUR_EMBED_URL"
  width="100%"
  height="180"
  allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture"
></iframe>
```

## Form behavior

The inquiry form currently opens the user's email app with all submitted details pre-filled.

This works without a backend and is perfect for a first GitHub Pages launch.

Later, you can connect it to:

- Formspree
- Netlify Forms
- Web3Forms
- A custom backend
- Supabase
- Firebase

## SEO note

Replace this line in `index.html` when you have your real domain:

```html
<link rel="canonical" href="https://example.com/" />
```

Use your final domain instead.
