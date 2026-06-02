# Apex Fraction-AI — Website

A complete static HTML/CSS website for Apex Fraction-AI Fractional IT Consultancy.

## File Structure

```
apex-fraction-ai/
├── index.html          Homepage
├── services.html       Services detail page
├── about.html          About page
├── experience.html     Career / experience timeline
├── contact.html        Contact form
├── privacy.html        Privacy policy
├── style.css           Shared design system & styles
├── assets/
│   └── apex-logo.png   Brand logo (add your file here)
└── README.md
```

## Before Going Live — Checklist

### 1. Add Your Logo
Copy your `Apex.png` logo file into the `assets/` folder and rename it `apex-logo.png`.

### 2. Update Contact Details
In `contact.html`, update:
- Email address (currently `hello@apexfractionai.co.uk`)
- Adjust to your actual domain once registered

### 3. Update the Privacy Policy
In `privacy.html`, replace all `[UPDATE...]` placeholders:
- `[UPDATE DATE BEFORE PUBLISHING]` → today's date
- `[YOUR DOMAIN]` → your website domain
- `[UPDATE WITH REGISTERED ADDRESS]` → your registered business address
- Update email addresses in the privacy page

### 4. Add Your Tagline
In `index.html`, locate this comment:
```html
<!-- TAGLINE PLACEHOLDER: Replace the paragraph above with your strapline when ready -->
```
Replace the paragraph above it with your finalised strapline.

### 5. Wire Up the Contact Form
The contact form in `contact.html` needs a backend to actually send emails.
Options (all have free tiers):

**Netlify Forms** (easiest if hosting on Netlify):
Add `netlify` attribute to the form tag and `data-netlify="true"`.

**Formspree** (works with any host):
1. Sign up at formspree.io
2. Create a form and get your endpoint URL
3. Change the form `action` attribute to your Formspree URL
4. Set `method="POST"`

**EmailJS** (sends from browser, no backend):
1. Sign up at emailjs.com
2. Connect your email account
3. Replace the `handleSubmit()` function with the EmailJS SDK call

### 6. Update Copyright Year
Footer shows `© 2025`. Update annually or make it dynamic.

---

## Deployment Options

### Option A: Netlify (Recommended — Free)
1. Go to [netlify.com](https://netlify.com) and create a free account
2. Drag and drop the entire `apex-fraction-ai/` folder into Netlify
3. Your site will be live at a `yoursite.netlify.app` URL immediately
4. Connect your own domain in the Netlify dashboard settings

### Option B: GitHub Pages (Free)
1. Create a GitHub account and a new repository
2. Upload all files to the repository
3. Go to Settings → Pages → Source → Deploy from branch (main)
4. Your site will be at `yourusername.github.io/reponame`
5. Add a custom domain in the Pages settings

### Option C: Traditional cPanel Hosting
1. Access your hosting control panel
2. Open File Manager → public_html directory
3. Upload all files (maintaining the folder structure)
4. `index.html` should be in the root of `public_html`
5. Create an `assets/` subfolder and upload your logo there

### Option D: Cloudflare Pages (Free, fast CDN)
1. Sign up at [pages.cloudflare.com](https://pages.cloudflare.com)
2. Connect your GitHub repository or upload directly
3. Configure your custom domain

---

## Custom Domain Setup
Once you have your domain (e.g. `apexfractionai.co.uk`):
1. Add it in your hosting provider's domain settings
2. Update your domain registrar's DNS to point to your host
3. Enable HTTPS/SSL (free via Let's Encrypt on most modern hosts)

---

## Fonts
The site uses Google Fonts:
- **Cormorant Garamond** — headings (authoritative, serif)
- **DM Sans** — body text (clean, professional)

These load from Google's CDN. For offline use, download them from [fonts.google.com](https://fonts.google.com) and host locally.

---

## Brand Colours
| Name       | Hex       | Usage                  |
|------------|-----------|------------------------|
| Navy Deep  | `#0f1e3d` | Hero backgrounds       |
| Navy       | `#1a2e5a` | Primary brand, headings |
| Navy Mid   | `#243a6e` | Gradients, cards       |
| Teal       | `#00b4c8` | Accent, CTA buttons    |
| Teal Dark  | `#008fa0` | Hover states           |
| Teal Light | `#4dd0c4` | Highlights             |
| Aqua       | `#00c9b1` | Gradient accents       |
