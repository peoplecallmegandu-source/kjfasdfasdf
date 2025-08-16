# Acme Studio — Static Multi-Page Site

This repository contains a small static website (HTML + Tailwind via CDN) with three pages:

- index.html — Home / landing page
- about.html — About, team and approach
- contact.html — Contact form with client-side validation and local draft saving

Design notes
- Full-width layouts: all main wrappers use w-full and max-w-none so the site fills the viewport width on all devices.
- Tailwind classes are used directly in the HTML for styling.
- Google Font: Inter is used. The font is referenced at the top of each HTML file (see HTML comments and link tags).
- No images are used anywhere (per request).
- Responsive and mobile-friendly layouts. Mobile menu toggle is included for small screens.
- Dark mode support is implemented using the class strategy (toggled via a button and persisted to localStorage).
- Subtle animations and hover effects applied with Tailwind utilities.

How to use
1. Open any of the HTML files in a modern browser (index.html is the entry point). No build step is required — Tailwind is loaded from the CDN.

2. Contact form behavior:
   - The contact form performs client-side validation and simulates a submission.
   - You can save a draft locally (saved to localStorage) and it will be preloaded on the contact page.

Files
- index.html — Landing page with hero, services, testimonials and CTA.
- about.html — Company mission, values, team and approach.
- contact.html — Contact form and company details.
- README.md — This file.

Customization
- To change the font, update the Google Fonts link in the head of the HTML files and adjust the inline style.
- To customize Tailwind configuration beyond the CDN defaults, consider switching to a local Tailwind build environment.

Notes
- All links between pages use relative paths (./about.html, ./contact.html).
- There are no external images; the site uses emoji and text-based UI elements only.

If you want additional pages, a CMS integration, or to export this to a static hosting provider, tell me how you'd like it hosted and I can provide deployment instructions or a build configuration.
