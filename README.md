# Two Brothers Lawn Service - Landing Page

A modern, high-performance, single-page landing site designed for a local landscaping and lawn care business. 

This project transforms a traditional print flyer into a premium digital experience, prioritizing clean aesthetics, smooth micro-interactions, and clear calls to action (CTAs).

## 🚀 Live Demo
*(You can add your GitHub Pages link here once deployed, e.g., `https://[your-username].github.io/two-brothers-lawn/`)*

## 🛠 Tech Stack
Designed for simplicity, speed, and zero build-step overhead. This project operates as a completely self-contained single file.
* **HTML5:** Semantic, accessible markup.
* **Tailwind CSS (via CDN):** For rapid, utility-first styling and responsive design.
* **GSAP & ScrollTrigger (via CDN):** For high-performance, scroll-based motion and staggered reveal animations.
* **Google Fonts:** Utilizing 'Inter' for crisp, highly legible typography.

## 🎨 Design Philosophy
The UI/UX is heavily inspired by the clean, neutral aesthetics of tech companies like Apple and Stripe:
* **Whitespace & Structure:** Ample padding and margins to let the content breathe and guide the user's eye naturally down the page.
* **Color Palette:** A professional, high-contrast slate/grayscale base, paired with targeted green accents to evoke nature and growth without overwhelming the layout.
* **Custom Iconography:** Inline, custom-designed SVG paths for standard services (Push Mower, String Trimmer, Edger, Blower) to keep HTTP requests low and visuals sharp.
* **Motion Design:** Elements are hidden on load to prevent Flash of Unstyled Content (FOUC). As the user scrolls, GSAP triggers smooth, staggered upward reveals, providing a premium feel without sacrificing performance.

## 📱 Features
* **Fully Responsive:** Adapts seamlessly from mobile devices to ultra-wide desktop monitors.
* **Quick Contact:** Direct `tel:` and `sms:` links implemented on primary buttons to drive immediate conversions from mobile users.
* **Single-File Architecture:** All HTML, CSS (Tailwind classes), and JavaScript (GSAP logic) live inside `index.html` for incredibly easy hosting and editing.

## 💻 Deployment
This project is static and can be hosted for free on platforms like **GitHub Pages**, **Vercel**, or **Netlify** simply by uploading the `index.html` file.
