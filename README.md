<img src="img/portfolio_screenshot.png"/>

# Personal Portfolio Template

A dark-mode, minimalist developer portfolio built with React, Tailwind CSS, and Framer Motion. No build tools required — open `index.html` in a browser and it works.

---

## Customization

All edits happen inside `index.html`. Search for each item below and replace it.

### 1. Your Name

Search for `Imtiaz Ahmed` — it appears in three places:

| Location | What to change |
|---|---|
| `<title>` tag | Browser tab title |
| `<meta>` tags | SEO / social previews |
| `<h1>` in the Hero section | The big heading on the page |

---

### 2. Your Bio & Location

Find the **About** section (`id="about"`). Update:

```
Comilla, Bangladesh  →  Your city, Country
CS student + freelancing  →  Your current role
```

Also update the four info rows:

```js
{ label: 'Location',  value: 'Comilla, Bangladesh 🇧🇩' },
{ label: 'Currently', value: 'CS student + freelancing' },
{ label: 'Interests', value: 'Minimalism, dev tools, open source' },
{ label: 'Learning',  value: 'Rust, system design, AI engineering' },
```

---

### 3. Your Projects

Find the `projects` array inside the **Work** section. Each project looks like this:

```js
{
  name: 'The Ledger',
  year: '2024',
  accentClass: 'ledger-accent',   // text color class (defined in <style>)
  barClass: 'ledger-bar',         // top color stripe class
  description: 'A smart personal finance tracker...',
  tags: ['Next.js', 'Prisma', 'Postgres', 'Stripe'],
  link: '#',                      // ← paste your live URL or GitHub link here
  custom: 1,                      // animation delay order, keep as-is
},
```

**To rename a project** — change `name`, `description`, `tags`, and `link`.

**To change a project's color** — find its accent + bar classes in the `<style>` block and update the hex values:

```css
.ledger-accent { color: #60a5fa; }   /* blue */
.ledger-bar    { background: linear-gradient(90deg, #1d4ed8, #3b82f6); }

.zetro-accent  { color: #c084fc; }   /* purple */
.zetro-bar     { background: linear-gradient(90deg, #7c3aed, #c084fc); }

.mouchak-accent { color: #fb923c; }  /* amber */
.mouchak-bar    { background: linear-gradient(90deg, #c2410c, #fb923c); }
```

**To add a 4th project** — copy any project object, paste it into the array, give it a new `accentClass`/`barClass` name, define those classes in `<style>`, and set `custom: 4`.

---

### 4. Your Tech Stack

Find the "Current stack" bento card and update the tags array:

```js
['Next.js 14', 'TypeScript', 'Tailwind CSS', 'Prisma', 'PostgreSQL', 'Framer Motion', 'Zustand', 'Vercel']
```

Also update the tech list in the Hero section:

```js
['Next.js', 'React', 'TypeScript', 'Tailwind', 'Node.js']
```

---

### 5. Contact & Social Links

Search for `mailto:imtiaz@example.com` — replace with your email (appears twice).

Update the social links at the bottom of the Contact section:

```js
{ label: 'GitHub',   href: 'https://github.com/YOUR_USERNAME' },
{ label: 'Twitter',  href: 'https://twitter.com/YOUR_HANDLE' },
{ label: 'LinkedIn', href: 'https://linkedin.com/in/YOUR_PROFILE' },
```

Also update the GitHub button in the Hero:

```html
<a href="https://github.com/YOUR_USERNAME" ...>GitHub</a>
```

---

### 6. Availability Status

The green dot at the top of the Hero says "Available for projects". Change or remove it:

```js
// To change the message:
<span className="font-mono text-xs text-[#52525b]">Available for projects</span>

// To hide it entirely, delete this motion.div block.
```

---

### 7. SEO & Meta Tags

Update these tags in `<head>`:

```html
<title>Your Name | Web Developer from Your Country</title>
<meta name="description" content="Your one-liner description." />
<meta name="keywords" content="Your Name, web developer, ..." />
<meta name="author" content="Your Name" />
<link rel="canonical" href="https://yoursite.com/" />
<meta property="og:title" content="Your Name | Web Developer" />
<meta property="og:description" content="Your tagline." />
```

---

### 8. Footer

```js
// Find this line and update both values:
<span className="font-mono text-xs">© 2024 Imtiaz Ahmed</span>
<span className="font-mono text-xs">Made in Bangladesh 🇧🇩</span>
```

---

## Deployment

This is a single HTML file with no build step. You can host it anywhere:

- **GitHub Pages** — push to a repo, enable Pages in Settings → Pages → Branch: `main`, folder: `/ (root)`
- **Vercel** — drag and drop the file at vercel.com/new
- **Netlify** — drag and drop at app.netlify.com/drop

---

## Tech Used

- [React 18](https://react.dev) via CDN
- [Tailwind CSS](https://tailwindcss.com) via CDN
- [Framer Motion 10](https://www.framer.com/motion/) via CDN
- [DM Sans + DM Mono](https://fonts.google.com) from Google Fonts

No npm. No bundler. No config. Just one file.

---

## License

MIT — use it, fork it, make it yours.
