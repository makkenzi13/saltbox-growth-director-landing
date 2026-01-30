# Saltbox Director of Growth Landing Page

A single-page landing page for Saltbox's Director of Growth role, designed as an interactive candidate assessment experience that embodies Saltbox's "capability over credentials" hiring philosophy.

## 🌐 Live Site

- **Production**: https://join-growth-director.saltbox.com
- **Render**: https://saltbox-growth-director-landing.onrender.com

## 📋 Project Overview

This isn't a traditional job posting—it's a candidate experience that:
- Introduces Saltbox's business model and values
- Explains the AI-native growth marketing role
- Presents a 4-step practical assessment challenge
- Provides a functional submission form with file uploads
- Sets clear expectations (24-hour review, 1-week hiring process)

### Key Philosophy

**"Capability over credentials"** — Saltbox evaluates what candidates can produce today with modern AI tools, not years of experience or brand-name employers.

## 🛠 Technologies Used

- **HTML5** - Single-page structure
- **CSS3** - All styles inline, no external stylesheets
  - CSS Grid & Flexbox for layouts
  - CSS animations (keyframes, transitions)
  - Custom CSS properties (CSS variables)
  - Responsive design with media queries
- **Vanilla JavaScript** - No frameworks or libraries
  - Intersection Observer API for scroll animations
  - Event listeners for interactivity
- **Google Fonts API** - Typography (Inter, Inter Tight, Besley)
- **Formspree** - Form backend for submissions
- **Git & GitHub** - Version control
- **Render** - Static site hosting with auto-deploy

### Why No Build Tools?

This project intentionally uses vanilla HTML/CSS/JS without frameworks or build steps to keep it:
- Simple to modify
- Fast to deploy
- Easy to understand
- No dependencies or build pipeline to maintain

## 📁 File Structure

```
/
├── index.html                      # Main landing page
├── thank-you.html                  # Post-submission success page
├── README.md                       # This file
├── .gitignore                      # Git ignore rules
├── assets/                         # Images and graphics
│   ├── logo-black.png              # Saltbox logo (dark)
│   ├── logo-white.png              # Saltbox logo (light)
│   ├── team-photo.jpg              # Team photo
│   ├── always-be-shipping.jpg      # Image break section
│   ├── sb-graphic-1.png            # Brand pattern (yellow starbursts)
│   ├── sb-graphic-2.png            # Brand pattern (light texture)
│   ├── sb-graphic-3.png            # Brand pattern (gray starbursts)
│   └── sb-graphic-4.png            # Brand pattern (circuit/connection)
├── Reference Documents/            # Project specs and source materials
│   ├── Director-of-Growth-Landing-Page-Build-Prompt.md
│   ├── JD.pdf
│   ├── Assessment Framework.pdf
│   └── Candidate Evaluation.pdf
└── Saltbox-Brand-Assets/          # Official brand guidelines
    ├── logos/
    ├── fonts/
    └── saltbox-brand-guidelines-ai.md
```

## 🎨 Design System

### Color Palette

```css
--black-100: #2A2B33;    /* Primary text, dark backgrounds */
--orange: #FDB706;       /* Accent color (use sparingly) */
--soft-yellow: #FAF7E3;  /* Warm section backgrounds */
--fog: #E3EDE5;          /* Cool section backgrounds */
--sage: #CADCD5;         /* Callout blocks, subtle accents */
--shadow: #344343;       /* Secondary text, dark sections */
--white: #FFFFFF;        /* White backgrounds, light text */
--black-80: #595E53;     /* Muted text */
--dust: #627678;         /* Tertiary text */
```

### Typography

- **Headlines**: Inter Tight (always with `letter-spacing: 2px`)
- **Body text**: Inter
- **Accent/Italic emphasis**: Besley Italic (for warmth)

### Visual Principles

- Generous whitespace for breathing room
- Section rhythm through alternating background colors
- Clean, modern, warm aesthetic
- Mobile-first responsive design
- CSS-only icons (no icon fonts or SVG libraries)

## ✨ Interactive Features

1. **Journey Line** - Fixed vertical line on left that fills with scroll progress
2. **Hero Visual** - Floating animated gradient shapes with brand graphic overlay
3. **3D Globe** - Animated spinning globe with ocean/continents
4. **Evaluation Cards** - Hover effects with 3D tilt and CSS-based icons
5. **Form Interactions** - Drag-and-drop file upload with visual feedback
6. **Scroll Animations** - Sections fade in as you scroll (Intersection Observer)
7. **Smooth Scroll** - Anchor links scroll smoothly to sections

## 📝 Form Submission (Formspree Integration)

### How It Works

1. Form submits directly to Formspree endpoint: `https://formspree.io/f/maqjagga`
2. Formspree processes the submission (including file uploads)
3. User redirected to `thank-you.html`
4. Saltbox team receives email notification with submission data

### Form Fields

- `name` (text, required)
- `email` (email, required)
- `attachment` (file, required) - Candidate's work submission
- `notes` (textarea, optional) - Additional context or links

### Formspree Configuration

**Current Settings:**
- Form enabled: ✅
- Submission archive: ✅ On
- CAPTCHA: ❌ Off (can be enabled for spam protection)
- Email notifications: Configured in Formspree dashboard
- Redirect URL: `https://saltbox-growth-director-landing.onrender.com/thank-you.html`

**To modify Formspree settings:**
1. Log into Formspree account
2. Navigate to "Growth Marketer Landing Page" form
3. Update settings as needed

## 🚀 Deployment

### Current Setup

**Hosting**: Render (Static Site)
**Auto-Deploy**: Enabled on `main` branch pushes
**Custom Domain**: `join-growth-director.saltbox.com`

### Deployment Process

1. Push commits to `main` branch
2. Render automatically detects changes
3. Site rebuilds (usually 1-2 minutes)
4. Live site updates

### Manual Deploy

If needed, trigger manual deploy via Render dashboard:
https://dashboard.render.com/static/srv-d5uftpfgi27c7396hvl0

### DNS Configuration

**Domain**: `join-growth-director.saltbox.com`
**Type**: CNAME
**Target**: `saltbox-growth-director-landing.onrender.com`

## 💻 Local Development

Since this is a static site with no build process:

### Option 1: Simple HTTP Server

```bash
# Using Python 3
python3 -m http.server 8000

# Using Python 2
python -m SimpleHTTPServer 8000

# Using Node.js (if you have npx)
npx http-server
```

Then open: http://localhost:8000

### Option 2: Open Directly

Simply open `index.html` in your browser. Note: Some features (like fonts) may not work properly without a server due to CORS restrictions.

### Making Changes

1. Edit `index.html` or `thank-you.html` directly
2. Refresh browser to see changes
3. Commit and push to deploy

```bash
git add .
git commit -m "Your commit message"
git push origin main
```

## 🧪 Testing Checklist

Before deploying changes:

- [ ] Test form submission with real file upload
- [ ] Check all links work correctly
- [ ] Verify responsive design on mobile (375px, 768px, 1024px)
- [ ] Test animations and scroll effects
- [ ] Validate HTML (https://validator.w3.org/)
- [ ] Check browser console for errors
- [ ] Test on multiple browsers (Chrome, Firefox, Safari)
- [ ] Verify images load correctly
- [ ] Confirm Formspree redirect works

## 📊 The Assessment Challenge

Candidates complete a 4-step assessment:

1. **Reverse-engineer Saltbox's growth engine** - Analyze public info, identify gaps
2. **Propose AI-powered initiative** - Specific 30-day project plan
3. **Present it** - Any format (deck, Notion, Loom, PDF)
4. **Show your work** - "How I Built This" appendix

**Expected time**: ~1 hour (flexible)

### Evaluation Criteria

1. **Depth of insight** - Non-obvious business understanding
2. **Strategic clarity** - Specific, actionable recommendations
3. **AI fluency** - Genuine understanding of modern tools
4. **Brand resonance** - Matches Saltbox's voice and values
5. **Execution quality** - Polished, professional presentation

## 💼 Compensation Details

- **Base**: $80K–$180K
- **Performance bonus**: Included
- **Stock options**: Included
- **Benefits**: Full medical, 401(k), parental leave, PTO, learning budget
- **Work model**: Remote-first (Eastern Time hours required)

## 🔧 Common Modifications

### Updating Form Endpoint

Edit the form action in `index.html`:

```html
<form id="submission-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST" enctype="multipart/form-data">
```

### Changing Colors

Update CSS variables in the `:root` selector:

```css
:root {
  --black-100: #2A2B33;
  --orange: #FDB706;
  /* etc */
}
```

### Adding New Sections

1. Copy an existing section structure
2. Update section number in `.section-num`
3. Add unique ID for anchor linking
4. Update any navigation links

### Modifying Globe Animation

Find the `.globe` and `@keyframes globeSpin` styles to adjust:
- Animation duration (currently 20s)
- Colors (ocean blue, land sage green)
- Size (currently 120px)

## 📚 Reference Documentation

- **Design Brief**: `Reference Documents/Director-of-Growth-Landing-Page-Build-Prompt.md`
- **Brand Guidelines**: `Saltbox-Brand-Assets/saltbox-brand-guidelines-ai.md`
- **Assessment Framework**: `Reference Documents/Assessment Framework.pdf`

## 🐛 Known Issues / Future Enhancements

- Form submission is standard POST (page navigation) - could be enhanced with AJAX for smoother UX
- Globe animation could use more sophisticated 3D rendering
- No reCAPTCHA currently (available via Formspree if needed)
- Could add analytics tracking (Google Analytics, Plausible, etc.)

## 📞 Support

**Questions about the landing page:**
- Repository: https://github.com/makkenzi13/saltbox-growth-director-landing
- Formspree Dashboard: https://formspree.io/forms/maqjagga
- Render Dashboard: https://dashboard.render.com/static/srv-d5uftpfgi27c7396hvl0

**Questions about the role:**
- Email: info@saltbox.com
- Website: https://saltbox.com/careers

## 📄 License

Proprietary - © Saltbox. All rights reserved.

---

Built with ❤️ for Saltbox by Claude Code
