# MS Studio — Premium Wedding Photography & Videography

A highly optimized, luxury single-page website built for a high-end cinematic wedding studio. Designed with an elegant "Ivory & Gold" aesthetic, this project focuses on high performance, smooth animations, and a premium user experience across all devices.

## 🌟 Key Features

### 🎨 Premium Design & Layout
* **Luxury Color Palette**: Warm ivory backgrounds (`#faf8f5`) with sophisticated gold accents (`#b8926a`) designed to evoke a romantic, editorial feel.
* **Boutique Typography**: Uses **Playfair Display** for elegant headings and **DM Sans** for highly legible, modern body copy.
* **Fully Responsive**: Flawless layout scaling from 4K desktop monitors down to mobile screens, featuring a custom mobile hamburger navigation menu.
* **Immersive Visuals**: An advanced CSS Grid portfolio masonry layout that beautifully showcases cinematic films and fine-art photography.

### ⚡ Extreme Performance Optimizations
* **Hardware-Accelerated Animations**: Smooth, 60-FPS interactions using `transform: scaleX()` and `translateY()` instead of layout-thrashing properties like `width` or `top`.
* **Intersection Observer API**: Replaced traditional (and laggy) scroll event listeners with modern Observers to trigger scroll-reveal animations and active navigation highlighting without dropping frames.
* **Jank-Free Scrolling**: Parallax `background-attachment: fixed` effects are intelligently disabled on mobile devices to prevent notorious iOS jittering. The hero background animation uses a scale-down technique to completely prevent image pixelation.

### 📱 Progressive Web App (PWA) Ready
* **Installable**: Users can add the website directly to their mobile home screens as a native app via the configured `manifest.json`.
* **Service Worker (`sw.js`)**: Configured for offline capabilities, ensuring the site loads blazing fast on repeat visits.
* **Themed Interface**: The mobile browser status bar automatically matches the brand's gold accent color.

## 🛠 Tech Stack

This project is intentionally built without heavy frameworks to maintain absolute control over the DOM and performance.

* **HTML5**: Semantic markup structured for accessibility and SEO.
* **Vanilla CSS3**: Custom design system using CSS Variables (`:root`), Flexbox, CSS Grid, and custom keyframe animations. FontAwesome integrated for vector icons.
* **Vanilla JavaScript (ES6)**: Lightweight logic for scroll tracking, mobile menu toggling, smooth scrolling (Back to Top), and Intersection Observers.

## 📂 Project Structure

```text
MS-studios/
├── index.html       # The main single-page application structure
├── style.css        # The complete design system and responsive media queries
├── sw.js            # Service worker for PWA functionality
├── manifest.json    # Web App Manifest for mobile installation
├── msstudio.png     # Main brand logo
└── README.md        # Project documentation
```

## 🚀 Getting Started

Because this is a vanilla front-end stack, no build steps or heavy `npm install` commands are required!

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/just-umar1/MS-studios.git
   ```
2. Open `index.html` directly in any modern web browser.
3. *Optional*: To test the Service Worker (PWA) functionality locally, serve the directory using a simple local web server (e.g., VS Code Live Server, or running `npx serve .` / `python3 -m http.server`).

## 🖌 Customization

To alter the primary branding, navigate to `style.css` and modify the CSS variables under the `:root` pseudo-class:

```css
:root {
    --bg: #faf8f5;           /* Main background */
    --text-dark: #2c2420;    /* Headings */
    --accent: #b8926a;       /* Primary brand color */
    --font-heading: 'Playfair Display', serif;
}
```

---
*Vibe-coded to perfection. Crafted with passion.*
