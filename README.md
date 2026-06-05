# SkyScale Media — Meta Ad Agency Landing Page

A premium, dark-themed landing page template for Meta (Facebook/Instagram) advertising agencies, media buyers, and digital marketing professionals. Built with pure HTML, CSS, and JavaScript — no build tools required.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![HTML](https://img.shields.io/badge/HTML-5-orange.svg)
![CSS](https://img.shields.io/badge/CSS-3-blue.svg)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow.svg)

---

## ✨ Features

| Feature | Description |
|---------|-------------|
| **3D Earth Globe** | Realistic rotating Earth with Three.js (clouds, atmosphere, specular lighting) |
| **Starfield Background** | Twinkling CSS stars + subtle Three.js particle stars in the hero |
| **Scroll Animations** | Intersection Observer-based fade-up animations throughout |
| **Infinite Marquees** | Smooth auto-scrolling logo strips, portfolio cards, and testimonials |
| **Mobile-First Responsive** | Fully optimized for mobile, tablet, and desktop |
| **FAQ Accordion** | Smooth expand/collapse with CSS transitions |
| **Sticky Navigation** | Glassmorphism navbar with blur backdrop |
| **Performance Optimized** | `will-change`, `transform` animations, minimal repaints |
| **Zero Dependencies** | Only Three.js loaded via CDN — everything else is vanilla |

---

## 📁 File Structure

```
skyscale-media-landing/
├── index.html          # Main landing page (single file)
├── README.md           # This file
├── LICENSE             # MIT License
├── .gitignore          # Git ignore rules
└── assets/             # (Optional) Create this folder for local images
    ├── images/
    └── fonts/
```

> **Note:** This template is intentionally a single `index.html` file so it's easy to host anywhere — GitHub Pages, Netlify, Vercel, or any static server.

---

## 🚀 Quick Start

### 1. Clone or Download
```bash
git clone https://github.com/YOUR_USERNAME/skyscale-media-landing.git
cd skyscale-media-landing
```

### 2. Open Locally
Simply open `index.html` in your browser, or use a local server:

```bash
# Python 3
python -m http.server 8000

# Node.js (if you have npx)
npx serve .

# PHP
php -S localhost:8000
```

Then visit `http://localhost:8000`

### 3. Deploy
Upload `index.html` to any static hosting service:
- [GitHub Pages](https://pages.github.com/)
- [Netlify Drop](https://app.netlify.com/drop)
- [Vercel](https://vercel.com/)
- [Cloudflare Pages](https://pages.cloudflare.com/)

---

## 🎨 Customization Guide (No Code Required)

You don't need to know how to code to edit this template. Just open `index.html` in any text editor (like Notepad, VS Code, or even online editors) and follow the guide below.

### Changing Text
Every piece of text is plain HTML inside the `<body>`. Simply find the text you want to change and replace it.

```html
<!-- Example: Change the headline -->
<h1>Scale Your Revenue With Meta Ads That Actually Work</h1>
```

### Changing Colors
All colors are defined as **CSS Variables** at the top of the `<style>` block:

```css
:root {
    --bg: #000000;              /* Main background */
    --surface: #0a0a0a;        /* Card backgrounds */
    --surface-light: #111111;  /* Lighter cards */
    --border: rgba(255,255,255,0.06); /* Borders */
    --text: #ffffff;            /* Main text */
    --text-secondary: #a1a1aa;  /* Subtitles */
    --text-muted: #71717a;      /* Descriptions */
    --accent: #3b82f6;          /* Blue accent */
    --accent-glow: rgba(59,130,246,0.3); /* Glow effect */
    --success: #22c55e;         /* Green badges */
}
```

Change any value and the entire site updates automatically.

### Changing Fonts
The template uses **Inter** from Google Fonts. To change it:
1. Replace the Google Fonts `<link>` in the `<head>`
2. Update the `font-family` in the `body` CSS rule

```html
<!-- Current font -->
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800;900&display=swap" rel="stylesheet">
```

### Changing Images
Replace the `data:image/svg+xml` placeholders with real image URLs:

```html
<!-- Before -->
<img src="data:image/svg+xml,<svg...>" alt="Campaign 1">

<!-- After -->
<img src="assets/images/your-image.jpg" alt="Campaign 1">
```

### Changing the 3D Globe
The globe is powered by **Three.js** and loads Earth textures from a CDN. To customize:
- **Size:** Adjust `.hero-earth-container` width/height in CSS
- **Rotation Speed:** Change `autoRotateAngle += 0.002;` in the JavaScript
- **Textures:** Replace the texture URLs in the `textureLoader.load()` calls
- **Remove it:** Delete everything inside `<script type="module">` and the `.hero-earth-container` div

### Changing Animation Speeds
Look for `@keyframes` and `animation-duration` values in the CSS:

```css
@keyframes slideLeft {
    from { transform: translateX(0); }
    to { transform: translateX(-50%); }
}

.scroller-track {
    animation: slideLeft 30s linear infinite; /* Change 30s to any value */
}
```

### Adding/Removing Sections
Each section is wrapped in a `<section>` tag with a class name:
- `class="hero"` — Hero section
- `class="services"` — Services grid
- `class="testimonials"` — Testimonials marquee
- `class="faq"` — FAQ accordion
- etc.

Copy-paste an entire `<section>...</section>` block to duplicate it, or delete the block to remove it.

---

## 📱 Sections Included

1. **Hero** — Headline, subheadline, CTA buttons, trust badge, 3D globe
2. **Logo Scroller** — Client/partner logos (infinite scroll)
3. **Typography Statement** — Bold mission statement with gradient text
4. **Portfolio** — Campaign showcase with hover overlays
5. **Services** — 4-card grid (Ad Management, Agency Accounts, PR, Facebook Assets)
6. **Platforms** — Social media platform icons (infinite scroll)
7. **Benefits** — 6-card value proposition grid
8. **Process** — 4-step vertical timeline
9. **Testimonials** — 8 client reviews in infinite marquee
10. **Results** — Key metrics (clients, ad spend)
11. **Founder** — Founder bio card
12. **FAQ** — 5-item accordion
13. **CTA** — Final call-to-action
14. **Footer** — Links, contact info, social icons

---

## 🛠️ For Developers

### External Dependencies (CDN)
| Resource | URL | Purpose |
|----------|-----|---------|
| Google Fonts | `fonts.googleapis.com` | Inter font family |
| Three.js | `unpkg.com/three@0.128.0` | 3D Earth globe |
| Earth Textures | `threejs.org/examples/textures/planets/` | Globe surface maps |

### Browser Support
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

> Three.js WebGL requires a modern browser with hardware acceleration enabled.

### Performance Notes
- The 3D globe renders at device pixel ratio (`window.devicePixelRatio`). On high-DPI mobile screens, you may want to cap this to `2` for better performance.
- All animations use `transform` and `opacity` for GPU compositing.
- Images are currently SVG placeholders — replace with optimized WebP/JPEG for production.

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

You are free to:
- ✅ Use it for personal or commercial projects
- ✅ Modify, distribute, and sublicense
- ✅ Sell it as part of a product or service
- ✅ Include it in templates or themes

Requirements:
- Include the original copyright notice
- Include the MIT License text

---

## 🙋 Support & Questions

If you or your subscribers have questions:
1. Check the **Customization Guide** section above
2. Open an [Issue](../../issues) on this repository
3. For private support, contact: skyscalemedia@gmail.com

---

## 📝 Changelog

### v1.0.0 — Initial Release
- Complete landing page with 14 sections
- Three.js 3D Earth globe with atmosphere and clouds
- Responsive design (desktop, tablet, mobile)
- FAQ accordion, infinite marquees, scroll animations
- Single-file architecture for easy deployment

---

**Built with ❤️ by SkyScale Media**
