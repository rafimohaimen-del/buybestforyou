# BuyBestForYou — Independent Buying Guide & Review Platform

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![Zero JS](https://img.shields.io/badge/JavaScript-Zero_Dependencies-success?style=for-the-badge)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![WCAG AA](https://img.shields.io/badge/Accessibility-WCAG_2.1_AA-blue?style=for-the-badge)](https://www.w3.org/WAI/standards-guidelines/wcag/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)

> **Live Demo**: [https://rafimohaimen-del.github.io/buybestforyou/>](https://rafimohaimen-del.github.io/buybestforyou/)  
> *(Update the URL above once you deploy to GitHub Pages!)*

A comprehensive, production-grade, responsive editorial buying-guide and product review website built with **100% Pure HTML5 and CSS3** (zero JavaScript, zero external CSS frameworks, zero runtime libraries). 

Engineered directly from **15 high-fidelity UI/UX design mockups** following rigorous accessibility standards (WCAG AA), custom design system tokens, and advanced CSS techniques.

---

## 🌟 Key Highlights & Engineering Features

- **⚡ Zero JavaScript Overhead**: 100% of the UI interactivity—including mobile sliding drawer menus, category dropdowns, sticky reading navigation, and collapsible FAQs—is achieved using pure CSS and semantic HTML5 APIs.
- **📱 Fully Responsive (Mobile-First)**: Pixel-precise layouts across mobile screens (375px+), tablets (768px+), laptops (1024px+), and high-resolution desktop viewports (1280px+).
- **♿ WCAG 2.1 AA Compliant**:
  - Primary CTA (`#B84A14`) achieves a **5.21:1** contrast ratio on white surfaces.
  - Secondary text (`#5B6470`) achieves **6.0:1** contrast ratio.
  - Full keyboard focus indicators (`outline: 2px solid #2563EB`).
  - Strict semantic landmark hierarchy (`<header>`, `<nav>`, `<main>`, `<article>`, `<section>`, `<aside>`, `<footer>`).
- **🎨 Modular CSS Architecture**: Decoupled into Design Tokens (`variables.css`), Layout Shell (`layout.css`), UI Components (`components.css`), and Page Grid Templates (`pages.css`).
- **📐 Interactive Pure CSS Patterns**:
  - **Mobile Drawer Nav**: Accessible CSS Checkbox Hack (`#nav-toggle:checked ~ .main-nav`).
  - **Collapsible FAQs**: HTML5 `<details>` and `<summary>` elements with animated SVG rotational chevrons.
  - **Sticky Reading Sidebar**: Pure CSS `position: sticky; top: 90px;` with smooth scrolling anchors.
  - **Mobile Sticky CTA Bar**: Viewport-anchored bottom action bar on mobile screens.
  - **Radial & Linear Meters**: Custom score badges (`4.6/5`), sentiment bars, and pros/cons callout cards.

---

## 🗂️ Complete Page Directory

| File | Template Type | Design Mockup Reference | Key Features |
| :--- | :--- | :--- | :--- |
| [`index.html`](index.html) | **Homepage** | `1 · Homepage.png` & `11 · Mobile homepage.png` | Hero search with instant tags, 4-category cards, Winners grid, Methodology dark section, Latest reviews |
| [`category.html`](category.html) | **Category Hub** | `2 · Category guide listing.png` | Faceted sidebar filtering (budget, rating, type), sort controls, article grid, pagination, FAQ accordion |
| [`review-roundup.html`](review-roundup.html) | **Best-of Roundup** | `3 · Review single.png` & `12 · Mobile review single.png` | Sticky Table of Contents, Quick Answer callout, comparison table, numbered award winners, mobile sticky CTA bar |
| [`product-single.html`](product-single.html) | **Single Product Review** | `4 · Product single.png` | Product photo gallery, overall score gauge (`4.6`), metric bars, sentiment breakdown, technical specs table |
| [`blog.html`](blog.html) | **Editorial Blog** | `5 · Blog listing.png` | Category pill navigation, 9-card responsive article grid, read-time chips, author bylines, pagination |
| [`blog-single.html`](blog-single.html) | **How-To Editorial Post** | `6 · Blog single.png` | Sticky section TOC, Short Answer box, step-by-step numbered instructions, inline product highlight callout |
| [`contact.html`](contact.html) | **Contact & Inquiries** | `7 · Contact (+ guest author).png` | Editorial inquiry form, error reporting, revenue disclosure, guest contributor callout banner |
| [`about.html`](about.html) | **About & Testing Method** | `8 · About + How we test.png` | Mission statement, "What we do / What we don't" split cards, 4-step testing methodology, editor persona profiles |
| [`disclosure.html`](disclosure.html) | **Affiliate Disclosure & Legal** | `9 · Legal page template.png` | Sticky legal TOC, Amazon Associate disclosure callout, editorial independence terms, privacy policy |
| [`404.html`](404.html) | **Custom 404 Error** | `10 · 404 + search.png` | Search recovery input, category quick pills, recommended guide cards |

---

## 🎨 Design System & CSS Token Specifications

All visual styles are grounded in the project foundation specifications:

### Core Color Palette
- **Brand Ink (Headings & Dark Elements)**: `#111827`
- **Body Text**: `#1F2937`
- **Muted / Secondary Text**: `#5B6470` (6.0:1 contrast ratio)
- **Primary CTA (Terracotta / Rust)**: `#B84A14` (5.21:1 contrast ratio)
- **CTA Hover State**: `#963B0E`
- **Trust Accent (Cobalt Blue)**: `#2563EB`
- **Border & Dividers**: `#E5E7EB`

### Category Tint Palette
- **Automotive**: Background `#FBF8F5` · Dot `#7A4E2D`
- **Electronics**: Background `#E6EFF4` · Dot `#2E6FA3`
- **Home Appliances**: Background `#EEF5F0` · Dot `#3A8452`
- **Health & Fitness**: Background `#FDF0F3` · Dot `#B23A5C`

---

## 🚀 How to Run Locally

Because this project is built entirely with vanilla HTML5 and CSS3, **no build steps, Node.js installations, or package managers are required!**

### Option 1: Direct File Opening
Double-click `index.html` in your file explorer to open it directly in any modern web browser (Chrome, Edge, Firefox, Safari).

### Option 2: Local HTTP Server (VS Code Live Server / Python)
To test smooth navigation and base URLs:
```bash
# Using Python 3:
python -m http.server 8000

# Open in your browser:
http://localhost:8000/
```

---

## 🌐 Deploy to GitHub Pages (Step-by-Step)

Follow these steps to host this site live on GitHub for free and get a portfolio URL:

1. **Initialize Git in this directory**:
   ```bash
   git init
   git add .
   git commit -m "feat: complete BuyBestForYou responsive HTML/CSS website"
   ```

2. **Create a new repository on GitHub**:
   - Go to [github.com/new](https://github.com/new).
   - Name your repository (e.g., `buybestforyou-website` or `buybestforyou`).
   - Keep it **Public** so GitHub Pages can host it for free.
   - Click **Create repository**.

3. **Link and push your code**:
   ```bash
   git remote add origin https://github.com/<your-username>/buybestforyou-website.git
   git branch -M main
   git push -u origin main
   ```

4. **Enable GitHub Pages**:
   - In your GitHub repository, go to **Settings** > **Pages** (in the left sidebar).
   - Under **Build and deployment > Source**, select **Deploy from a branch**.
   - Under **Branch**, choose `main` and `/ (root)`, then click **Save**.
   - Wait 1–2 minutes. GitHub will provide your live URL:  
     `https://<your-username>.github.io/buybestforyou-website/`

---

## 💼 How to Showcase on Your Portfolio & Resume

Add this project to your developer portfolio, LinkedIn, or CV using the template below:

### Project Card Description
> **BuyBestForYou — Semantic & Responsive E-Commerce Buying Guide**  
> *Tech Stack*: HTML5, CSS3, Responsive Web Design, WCAG 2.1 AA Accessibility  
> *Live Link*: `https://<your-username>.github.io/buybestforyou-website/`  
> *GitHub Repo*: `https://github.com/<your-username>/buybestforyou-website`  
>
> - Engineered a 10-page, zero-JavaScript editorial website matching 15 high-fidelity UI design mockups.
> - Implemented interactive UI components (mobile drawer navigation, collapsible accordions, sticky reading sidebars) strictly using HTML5 semantics and CSS3.
> - Enforced WCAG 2.1 AA color contrast compliance (5.21:1 on primary CTAs, 6.0:1 on secondary text) and keyboard accessibility.
> - Structured clean, modular CSS token architecture across layouts, components, and responsive media queries.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
