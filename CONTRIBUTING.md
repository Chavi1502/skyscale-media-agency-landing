# Contributing to SkyScale Media Landing Page

Thank you for your interest in improving this template! Whether you're fixing a bug, adding a feature, or improving documentation, your contributions are welcome.

## How to Contribute

### 1. Fork the Repository
Click the "Fork" button on GitHub to create your own copy.

### 2. Clone Your Fork
```bash
git clone https://github.com/YOUR_USERNAME/skyscale-media-landing.git
cd skyscale-media-landing
```

### 3. Create a Branch
```bash
git checkout -b feature/your-feature-name
```

### 4. Make Your Changes
- Edit `index.html` directly for content changes
- Edit CSS inside the `<style>` block in `index.html`
- Edit JavaScript inside the `<script>` blocks in `index.html`

### 5. Test Your Changes
- Open `index.html` in Chrome, Firefox, and Safari
- Test on mobile (use browser DevTools device emulation)
- Verify the 3D globe loads correctly
- Check that all animations still work

### 6. Commit and Push
```bash
git add index.html
git commit -m "feat: add [description of change]"
git push origin feature/your-feature-name
```

### 7. Open a Pull Request
Go to the original repository and click "New Pull Request". Describe what you changed and why.

## What We're Looking For

- 🐛 **Bug fixes** — responsive issues, animation glitches, broken links
- 🎨 **Design improvements** — better spacing, typography, color accessibility
- ⚡ **Performance** — faster load times, reduced bundle size, better lazy loading
- ♿ **Accessibility** — ARIA labels, keyboard navigation, color contrast
- 🌍 **Localization** — making the template easier to translate

## What to Avoid

- ❌ Adding heavy dependencies (keep it lightweight)
- ❌ Breaking existing customization patterns
- ❌ Removing sections without a good reason
- ❌ Changing the single-file architecture (unless discussed first)

## Code Style

- Use 4 spaces for indentation inside HTML/CSS/JS
- Keep CSS variables in `:root` for easy theming
- Use semantic HTML tags (`<section>`, `<article>`, `<nav>`)
- Comment complex animations or JavaScript logic

## Questions?

Open an [Issue](../../issues) if you're unsure about anything. We're happy to help!
