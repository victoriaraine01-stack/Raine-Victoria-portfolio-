# Portfolio – Project README

A personal portfolio landing page built with **vanilla HTML, CSS, and JavaScript** — no frameworks, no dependencies, no internet required to run.

---

## Folder Structure

```
portfolio/
├── index.html              ← Entry point — open this in a browser
└── assets/
    ├── css/
    │   └── style.css       ← All styles
    ├── js/
    │   └── script.js       ← All interactivity
    ├── images/
    │   ├── project-ecommerce.svg   ← Placeholder (replace with your image)
    │   ├── project-portfolio.svg   ← Placeholder (replace with your image)
    │   └── project-mobile.svg      ← Placeholder (replace with your image)
    └── icons/
        ├── icon-code.svg
        ├── icon-palette.svg
        ├── icon-zap.svg
        ├── icon-github.svg
        ├── icon-linkedin.svg
        ├── icon-twitter.svg
        ├── icon-mail.svg
        └── icon-external-link.svg
```

---

## How to Run

**No server, no install needed.**  
Just double-click `index.html` — it opens directly in any web browser.

---

## How to Customise

### Change Your Name
Open `index.html` and find/replace `Dan` with your own name.  
Also update the `<title>` tag inside `<head>`.

### Replace Project Images

1. Save your image as a JPEG or PNG (recommended: **800 × 480 px**).
2. Place it inside `assets/images/`.
3. Open `assets/js/script.js` and update the `image:` path for each project:

```js
// Before
image: 'assets/images/project-ecommerce.svg',

// After (example)
image: 'assets/images/my-shop-screenshot.jpg',
```

### Add a New Project

Open `assets/js/script.js` and add a new object to the `projects` array:

```js
{
  title: 'My New Project',
  description: 'A short description of what this project does.',
  image: 'assets/images/my-new-project.jpg',
  tags: ['HTML', 'CSS', 'JavaScript'],
  link: 'https://myproject.com'
}
```

### Update Social Links

Open `index.html`, find the `<!-- Social Links -->` section in the footer,
and replace each `href="#"` with your real profile URL:

```html
<a href="https://github.com/yourusername" ...>
<a href="https://linkedin.com/in/yourprofile" ...>
```

### Replace Icons

The icons in `assets/icons/` are plain SVG files — text files you can open in any editor.  
Sites to find free SVG icons:
- [heroicons.com](https://heroicons.com) (same style as these icons)
- [feathericons.com](https://feathericons.com)
- [iconsvg.xyz](https://iconsvg.xyz)

Download an icon, save it to `assets/icons/`, and update the `src` in `index.html`.

---

## Week 9 — Adding Bootstrap

When you're ready to integrate Bootstrap:

1. Add the Bootstrap CDN link in `<head>` (above your own `style.css`):
   ```html
   <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" />
   ```
2. Replace custom CSS class names with Bootstrap utility classes one section at a time.
3. Your own `style.css` overrides Bootstrap — so you can mix both.

## Week 9 — Adding Tailwind CSS

1. Add the Tailwind CDN play script in `<head>`:
   ```html
   <script src="https://cdn.tailwindcss.com"></script>
   ```
2. Replace class names in `index.html` with Tailwind utilities.
3. Remove the now-unused rules from `style.css`.

---

## Key Concepts in This Project

| File | Concept |
|------|---------|
| `index.html` | Semantic HTML5, ARIA attributes, relative file paths, SEO meta tags |
| `assets/css/style.css` | CSS custom properties, Flexbox, Grid, media queries, animations |
| `assets/js/script.js` | DOM selection, event listeners, functions, array `.forEach`, template literals |
| `assets/icons/*.svg` | SVG file format, loading local files with `<img src="">` |
| `assets/images/*.svg` | Placeholder assets, `object-fit: cover`, `loading="lazy"` |
