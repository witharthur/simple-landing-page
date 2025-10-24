# Elevate Labs — Responsive Landing Page

## Overview

This project is a **responsive landing page** built with pure **HTML and CSS**. It demonstrates the use of **semantic HTML5 elements**, **Flexbox**, **CSS Grid**, and **CSS variables** for a modern, clean design. The design also includes a **forum/comment section** and contact form for user interactions.

## Features

* Fully **responsive layout** using mobile-first approach.
* **CSS variables** defined under `:root` for easy theming:

```css
:root{
  --bg: #0f172a;
  --bg-soft: #111827;
  --text: #e5e7eb;
  --muted: #cbd5e1;
  --brand: #7c3aed;
  --brand-600:#6d28d9;
  --panel:#0b1220;
  --card:#111827;
  --border: rgba(255,255,255,.08);
  --shadow: 0 10px 30px rgba(0,0,0,.25);
}
```

* Sticky header with **collapsible hamburger menu** for mobile devices.
* **Hero section** with radial gradients and responsive typography.
* **Features grid** using CSS Grid that adapts to screen width.
* **About section** with bullets and alternative background.
* **Forum/comment section** styled for user posts.
* **Contact section** with email and form for inquiries.
* Footer with social links and copyright.

## How it Works

* **CSS Variables:** Allow easy customization of colors, shadows, and card styles.
* **Media Queries:** Adjust layout at breakpoints `768px`, `900px`, and `560px` for different devices.
* **Flexbox:** Used for header, buttons, and form alignment.
* **CSS Grid:** Used for features section and forum posts.
* **Responsive Images & Buttons:** Scales properly on mobile devices.

## How to Use

1. Clone the repository.
2. Open `index.html` in a browser.
3. Resize the browser window or use DevTools to test responsiveness.
4. Edit CSS variables in `:root` to change the theme.

## Key Concepts

* **Media Queries:** Apply CSS based on screen size.
* **Mobile-first Design:** Start with small screens and scale up.
* **Viewport Meta Tag:** Ensures proper scaling on mobile devices.
* **Flexbox & Grid:** For responsive layout structure.
* **Relative Units:** Use `%`, `rem`, `vw`, `vh` for fluid sizing.

## Submission Instructions

* Push all files to a new **GitHub repository**.
* Include `index.html`, `style.css`, and this `README.md`.
* Optionally, add screenshots.
* Submit the repository link before the deadline.

## Tips

* Test on multiple devices or browser simulators.
* Keep code semantic and accessible.
* Use DevTools to debug overflow or alignment issues.
