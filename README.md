# 🌐 Veeksha — Portfolio Website

A fully responsive personal portfolio and resume website built with plain HTML, CSS, and JavaScript. No frameworks, no dependencies — just open `index.html` and it works.

---

## 🚀 How to Run

No installation needed.

```bash
# Just open the file in your browser
double-click index.html
```

Or serve it locally with VS Code's **Live Server** extension for auto-reload during development.

---

## ✨ Features

- **Sticky Navbar** — smooth scroll to all sections, mobile hamburger menu
- **Hero Section** — animated availability badge, CTA buttons
- **About Section** — stats, bio, and skill tags
- **Skills Section** — categorised skill cards (Frontend, Backend, Database, Tools)
- **Projects Section** — project cards with tags and links
- **Contact Form** — JS validation (required fields, email format, min length); submissions saved to `localStorage` as JSON with timestamps
- **Admin Panel** — hidden by default; accessible via footer link
  - Password-protected login
  - Show / hide password toggle
  - Dynamically renders all contact form responses with timestamps
  - Logout returns to login screen
- **Dark / Light Theme** — toggle persists across sessions via `localStorage`

---

## 🗂️ File Structure

```
portfolio/
├── index.html      # Everything in one file (HTML + CSS + JS)
└── README.md
```

If with separate files:

```
portfolio/
├── index.html
├── css/
│   └── custom.css
├── js/
│   └── main.js
├── assets/
│    └── images/
└── README.md
```

---

## 🔐 Admin Access

1. Scroll to the footer and click **⚙ Admin**
2. Enter password
3. View all contact form submissions with timestamps
4. Click **Logout** to return to the login screen

> To change the password, update `ADMIN_PASSWORD` in the `<script>` section of `index.html`.

---

## 💾 localStorage Keys

| Key | Contents |
|-----|----------|
| `portfolio-theme` | `"light"` or `"dark"` |
| `portfolio_responses` | JSON array of contact form submissions |

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| Markup | HTML5 (semantic tags) |
| Styling | CSS3 (custom properties, Grid, Flexbox) |
| Logic | JavaScript (ES6+) |
| Fonts | Google Fonts (Manrope + Libre Baskerville) |
| Storage | Browser localStorage |

---

## ♿ Accessibility

- Semantic HTML (`<header>`, `<main>`, `<section>`, `<article>`, `<footer>`)
- `alt` attributes on all images
- Keyboard-navigable form and nav links
- Sufficient colour contrast in both light and dark themes
- Focus-visible states on interactive elements

---