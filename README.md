# Personal Portfolio Website

A dark, minimalist, and fully responsive portfolio website inspired by modern designer portfolios.

## Features

- **Dark minimalist design** - Black, white, and gray color scheme
- **Disappearing/reappearing header** - Navigation hides when scrolling down, shows when scrolling up
- **Floating social sidebar** - Social media icons fixed to the left side
- **Clean typography** - Professional and readable
- **Fully responsive** - Works perfectly on all devices
- **Easy to customize** - Clear structure with helpful comments

## Quick Start

1. **Open `index.html`** in any text editor
2. **Customize your information** (see sections below)
3. **Open `index.html` in your browser** to preview

That's it! No build tools, no installation needed.

## Customization

### Your Information (index.html)

The site is already set up with your information. Here's what's pre-filled:

- **Name:** Hriday Burra
- **Title:** Software Engineer
- **Email:** hriday.burra@gmail.com
- **LinkedIn:** https://www.linkedin.com/in/hriday-burra-bbb903283
- **GitHub:** https://github.com/daygthb

#### To Update Content:

**Projects (lines 73-145):**
- Project Alpha, Cloud Dashboard, Machine Learning Pipeline
- Edit project descriptions, technologies, and links
- Add more projects by copying a `<article class="project-card">...</article>` block

**Experience (lines 147-218):**
- Three positions pre-configured (Software Engineer, Backend Developer, Intern)
- Update job titles, dates, and bullet points with your actual experience
- Add more positions by copying a `<div class="timeline-item">...</div>` block

**About (lines 59-67):**
- Edit this paragraph with your personal story
- What drives you, your interests, your philosophy

**Education (lines 220-236):**
- Currently set for UC Davis
- Update with your school, degree, graduation date, and details

### Changing Colors

Open **styles.css** and modify the CSS variables at the top (lines 1-11):

```css
:root {
    --bg-primary: #0a0a0a;      /* Main background (very dark) */
    --bg-secondary: #111111;    /* Alternate section background */
    --bg-tertiary: #1a1a1a;     /* Card backgrounds */
    --text-primary: #ffffff;    /* Main text color */
    --text-secondary: #a0a0a0;  /* Secondary text */
    --text-muted: #666666;      /* Muted/decorative text */
    --accent: #ffffff;          /* Accent color */
    --border-light: #2a2a2a;    /* Border colors */
}
```

To lighten or change the color scheme, simply replace the hex codes.

### Removing the Floating Social Sidebar

If you don't want the fixed sidebar with social icons:
1. Open `index.html`
2. Delete lines 8-15 (the `<aside class="social-sidebar">...</aside>` block)

### Adjusting the Timeline Design

The timeline uses a simple vertical line. To remove the dotted line, delete the `timeline::before` styles in `styles.css` (lines 142-146).

## Design Details

### Disappearing Header
The navigation bar automatically hides when you scroll down and reappears when you scroll up. This is controlled by JavaScript in `script.js` (lines 1-25).

### Floating Social Sidebar
Fixed social media icons on the left side of the screen (desktop only). They disappear on mobile for a cleaner experience.

### Minimalist Aesthetic
- Dark background with subtle borders
- No heavy shadows or gradients
- Clean typography with good spacing
- Subtle hover effects

## Deployment

### GitHub Pages (Free)
1. Create a new repository on GitHub
2. Upload all files (`index.html`, `styles.css`, `script.js`)
3. Go to Settings → Pages
4. Select branch: main, folder: / (root)
5. Save and wait a few minutes
6. Your site: `https://yourusername.github.io/repo-name/`

### Netlify (Free & Fast)
1. Go to [netlify.com](https://netlify.com)
2. Drag and drop your project folder
3. Instantly get a live URL with HTTPS

### Vercel (Free)
1. Go to [vercel.com](https://vercel.com)
2. Sign up with GitHub
3. Import your repository or drag & drop folder
4. Auto-deploys on changes

## Files Structure

```
portfolio/
├── index.html      # Main HTML - edit your info here
├── styles.css      # All styling - customize colors here
├── script.js       # Interactivity (scroll effects, mobile menu)
└── README.md       # This file
```

## Mobile Responsiveness

- **Desktop (>768px):** Floating sidebar visible, full navigation
- **Tablet (768px):** Sidebar smaller, navigation as-is
- **Mobile (<768px):** Sidebar hidden, hamburger menu
- **Small Mobile (<480px):** Optimized spacing and font sizes

## Browser Support

All modern browsers (Chrome, Firefox, Safari, Edge) - fully tested.

## Want to Customize Further?

The code is clean and well-commented. To add sections:
1. Add a `<section id="section-name" class="section">...</section>` in `index.html`
2. Add corresponding link in the navigation menu
3. Style as needed in `styles.css`

Need help? The code is straightforward - just follow the patterns already in place!
