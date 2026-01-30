# Saltbox Director of Growth Landing Page

## Project Overview

This is a single-page landing page for Saltbox's Director of Growth role. It's designed as a candidate assessment experience that embodies Saltbox's philosophy of hiring for capability over credentials.

## What This Page Does

Rather than a traditional job posting, this page:
- Introduces candidates to Saltbox's business model and values
- Explains the Director of Growth role (AI-native growth marketing)
- Presents a 4-step practical assessment challenge
- Encourages AI usage and modern tool leverage
- Provides a submission form for candidates to upload their work
- Sets expectations for a fast hiring process (24-hour review, 1-week total)

## Key Philosophy

**"Capability over credentials"** — Saltbox doesn't care about years of experience or brand-name employers. They want to see what candidates can produce today with modern AI tools.

## File Structure

```
/
├── index.html                      # Main landing page (working version)
├── README.md                       # This file
├── assets/                         # Images used in the page
│   ├── logo-black.png
│   ├── logo-white.png
│   ├── team-photo.jpg
│   ├── always-be-shipping.jpg
│   └── [other graphics]
├── Reference Documents/            # Source materials and specs
│   ├── Director-of-Growth-Landing-Page-Build-Prompt.md
│   ├── JD.pdf
│   ├── Assessment Framework.pdf
│   └── Candidate Evaluation.pdf
└── Saltbox-Brand-Assets/          # Official brand assets
    └── [logo variations, guidelines]
```

## Design System

**Colors:**
- Black 100: `#2A2B33` (primary text)
- Orange: `#FDB706` (accent, used sparingly)
- Soft Yellow: `#FAF7E3` (warm backgrounds)
- Fog: `#E3EDE5` (cool backgrounds)
- Sage: `#CADCD5` (callout blocks)
- Shadow: `#344343` (secondary text, dark sections)
- White: `#FFFFFF`

**Typography:**
- Headlines: Inter Tight (with +2px letter-spacing)
- Body: Inter
- Accent/Italic emphasis: Besley Italic

**Visual Principles:**
- Generous whitespace
- Section rhythm through alternating background colors
- Clean, modern, warm aesthetic
- Fully responsive design

## Interactive Features

- Fixed journey line on left that fills as you scroll
- Floating animated shapes in hero section
- Hover effects on evaluation cards
- Smooth scroll navigation
- Form with drag-and-drop file upload
- Responsive breakpoints for mobile/tablet

## The Assessment Challenge

Candidates are asked to:
1. **Reverse-engineer Saltbox's growth engine** — Map positioning and identify gaps
2. **Propose an AI-powered initiative** — Specific, 30-day project plan
3. **Present it** — Any format (deck, Notion, Loom, PDF)
4. **Show your work** — "How I Built This" appendix with tools and process

Expected time: ~1 hour (but no strict limit)

## Evaluation Criteria (5 Dimensions)

1. Depth of insight
2. Strategic clarity
3. AI fluency
4. Brand resonance
5. Execution quality

## Compensation

- Base: $120K–$180K
- Performance bonus
- Full medical, 401(k), parental leave, PTO, learning budget
- Remote-first (Eastern Time hours required)

## Technical Notes

- Self-contained single HTML file
- All CSS inline in `<style>` tag
- All JavaScript inline in `<script>` tag
- Google Fonts CDN for typography
- Form submission currently shows success message (no backend connected)

## Next Steps for Deployment

When ready to deploy:
1. Connect form to backend (Netlify Forms, Formspree, or custom endpoint)
2. Host on Render as static site (or any static host)
3. Custom domain setup if needed
4. Test all interactive features and form submission
5. Verify mobile responsiveness

## Status

Current version is production-ready for review. Form needs backend integration before live deployment.
