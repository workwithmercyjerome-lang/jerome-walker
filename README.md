# Jerome Walker — Fitness Tracking Landing Page

A single-file, responsive landing page for a fitness tracking app, built with plain HTML5, CSS3,flexbox/grid, media queries and vanilla JavaScript. No frameworks, no build step — open the file and it runs.

 Live demo: (see [Deployment](#deployment) below)_

 https://workwithmercyjerome-lang.github.io/jerome-walker/
---

## Overview

Jerome Walker is a fitness-tracking product. This project is its marketing landing page: a header/nav, hero section, features grid, a dashboard "showcase" section, testimonials, a call-to-action, and a footer — all in one `index.html` file with embedded CSS and JS.

The design direction is a monochrome, premium fitness identity (black / off-white with a single lime accent used sparingly), paired with the Manrope and Inter typefaces for a clean editorial feel.

## Features

- **Responsive layout** — fluid across mobile, tablet, and desktop using CSS Grid, Flexbox, and `clamp()` for type scaling, with dedicated breakpoints at 1024px and 767px.
- **Sticky, blurred navigation** with a hamburger menu on mobile and a border/shadow that appears once the page is scrolled.
- **Hero section** with a headline, supporting copy, dual CTAs, and live-looking stat counters.
- **Features grid** (4 cards) with icon, title, and description, each animating into view on scroll.
- **Dashboard showcase** — a dark section with a mock activity ring, weekly bar chart, and goal-completion ring, built with pure CSS (conic-gradient rings, no chart library).
- **Testimonials** with star ratings and avatars.
- **Call-to-action band** and a multi-column footer with social links.
- **Interactivity**: mobile nav toggle, smooth in-page scrolling, toast notifications on button clicks, and scroll-triggered reveal animations via `IntersectionObserver`.
- **Accessibility touches**: semantic landmarks, `aria-label`/`aria-expanded` on interactive controls, visible `:focus-visible` states, alt text on images, and a `prefers-reduced-motion` override.
- **SEO/social basics**: meta description, Open Graph and Twitter card tags, and an inline SVG favicon.

## Technologies Used

- **HTML5** — semantic markup (`header`, `main`, `section`, `footer`, `nav`)
- **CSS3** — custom properties (design tokens), Flexbox, Grid, `clamp()`, `conic-gradient`, media queries
- **Vanilla JavaScript (ES6)** — no dependencies; handles the mobile menu, smooth scroll, toast messages, and scroll-reveal animations
- **Google Fonts** — Manrope (display) and Inter (body/data)

No build tools, package managers, or frameworks are required.

## Project Structure

```
.
├── index.html          # Markup, <style>, and <script> in one file
├── assets/
│   └── images/
│       ├── logo.jpg    # Brand logo (used in header + footer)
│       └── hero.png    # Hero section photo
└── README.md


## Setup Instructions

This is a static, dependency-free page, so there's nothing to install.

1. **Clone the repository**
   ```bash
   git clone https://github.com/<workwithmercyjerome-lang>/<jerome-walker>.git
   cd <jerome-walker>
   ```
2. **Open it locally** — either:
   - double-click `index.html` to open it directly in a browser, or
   - serve it locally so relative paths and browser dev tools behave normally:
     ```bash
     # Python
     python3 -m http.server 8080
     # then visit http://localhost:8080

     # or, with Node
     npx serve .
     ```
3. **Edit** — all styles live in the `<style>` block and all behavior in the `<script>` block at the bottom of `index.html`. Design tokens (colors, spacing, radii) are defined once as CSS custom properties at the top of the stylesheet in `:root`, so a full re-theme only touches a handful of lines.

## Deployment

- **GitHub Pages**:
- https://github.com/workwithmercyjerome-lang

- https://workwithmercyjerome-lang.github.io/jerome-walker/
