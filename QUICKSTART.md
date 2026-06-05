# Quick Start Guide for Subscribers

> **No coding skills required.** This guide will show you how to edit and publish this landing page in under 10 minutes.

---

## Option 1: Edit Online (Easiest)

### Using GitHub's Web Editor
1. Go to your repository on GitHub
2. Click on `index.html`
3. Click the **pencil icon** (✏️) in the top right to edit
4. Make your changes (see "What to Edit" below)
5. Scroll down, add a commit message like "Updated headline and colors"
6. Click **Commit changes**

### Using GitHub Codespaces (Free)
1. On your repository, click the **green "Code" button**
2. Select the **"Codespaces"** tab
3. Click **"Create codespace on main"**
4. A VS Code editor opens in your browser
5. Click `index.html` in the left sidebar
6. Edit and save (Ctrl+S or Cmd+S)
7. Changes are automatically saved to your repository

---

## Option 2: Edit on Your Computer

### Windows
1. Download the repository as a ZIP file (green "Code" button → "Download ZIP")
2. Extract the ZIP file
3. Right-click `index.html` → **Open with** → **Notepad** (or download [VS Code](https://code.visualstudio.com/))
4. Make your changes
5. Save the file (Ctrl+S)
6. Double-click `index.html` to open it in your browser and preview

### Mac
1. Download the repository as a ZIP file
2. Extract the ZIP file
3. Right-click `index.html` → **Open With** → **TextEdit**
4. Make your changes
5. Save (Cmd+S)
6. Double-click `index.html` to preview in Safari

---

## Option 3: Use a Free Website Builder Integration

### Publish on GitHub Pages (Free Hosting)
1. In your repository, go to **Settings**
2. Scroll down to **Pages** (left sidebar)
3. Under "Source", select **Deploy from a branch**
4. Select **main** branch and **/(root)** folder
5. Click **Save**
6. Wait 2-3 minutes
7. Your site will be live at `https://yourusername.github.io/skyscale-media-landing`

### Publish on Netlify (Free + Custom Domain)
1. Go to [netlify.com](https://netlify.com) and sign up (free)
2. Drag and drop your `index.html` file onto the Netlify dashboard
3. Your site is live instantly
4. Go to **Site settings** → **Domain management** to add a custom domain

---

## What to Edit (Cheat Sheet)

| What You Want to Change | Where to Find It | Look For |
|------------------------|------------------|----------|
| **Company name** | Top of file | `SkyScale Media` |
| **Hero headline** | Inside `<section class="hero">` | `<h1>Scale Your Revenue...` |
| **Hero subtitle** | Below the headline | `<p class="hero-subtitle">` |
| **Button text** | Near the headline | `Book Free Strategy Call` |
| **Phone number** | Footer section | `+91 81003 32427` |
| **Email** | Footer section | `skyscalemedia@gmail.com` |
| **Address** | Footer section | `P 285, Darga Road...` |
| **Colors** | Top of `<style>` block | `:root { --bg: #000000... }` |
| **Fonts** | `<head>` section | `fonts.googleapis.com` link |
| **Testimonials** | `<section class="testimonials">` | Multiple `.testimonial-card` blocks |
| **Services** | `<section class="services">` | `.service-card` blocks |
| **FAQ questions** | `<section class="faq">` | `.faq-question` spans |
| **Social links** | Footer | `href="#"` inside `.social-icon` |

---

## Common Issues & Fixes

### "The page looks blank or broken"
- Make sure you didn't accidentally delete a `<` or `>` symbol while editing
- Check that all quotes `"` are properly closed
- If unsure, download a fresh copy and compare

### "The 3D globe doesn't show"
- You need an internet connection (Three.js loads from a CDN)
- Try a different browser (Chrome works best)
- If it still doesn't work, the globe section can be safely removed

### "I want to remove a section entirely"
- Find the section by its class name (e.g., `<section class="founder">`)
- Select everything from `<section` to `</section>`
- Delete it
- Save and refresh your browser

### "Images are missing"
- The template uses placeholder SVG images
- Replace `src="data:image/svg+xml..."` with `src="your-image.jpg"`
- Upload your images to the same folder as `index.html`

---

## Need Help?

- 📧 Email: skyscalemedia@gmail.com
- 🐛 Open an issue on this GitHub repository
- 💬 Contact the template author through your subscription platform

---

**Happy customizing! 🚀**
