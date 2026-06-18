# UrbanDrip Clothing — Website Project

A multi-page streetwear clothing website built with HTML and CSS.

---

## Pages

| File | Description |
| `index.html` | Home page with hero banner and featured products |
| `about.html` | About the brand |
| `contact.html` | Contact form and info |
| `New arrivals.html` | Latest product drops |
| `Details.html` | Full product listing |

---

## File Structure

```
urbandrip/
├── index.html
├── about.html
├── contact.html
├── New arrivals.html
├── Details.html
├── style.css          ← single shared stylesheet
└── README.md
```

---

## CSS Overview (`style.css`)

All pages share one stylesheet. It is organized into sections:

1. **CSS Variables** — colours, fonts, spacing defined in one place using `:root`
2. **Reset & Base** — removes default browser margins/padding
3. **Layout Structure** — `.container` and `section` rules for consistent page width
4. **Header & Nav** — sticky header with hover effects
5. **Hero Section** — full-width banner with large heading
6. **Product Grid** — 3-column grid that collapses on smaller screens
7. **Cards** — product card styling with hover lift effect
8. **Text Sections** — used by About and Contact pages
9. **Contact Form** — input and button styling
10. **Footer** — simple dark footer
11. **Responsive Design** — media queries at 768px (tablet) and 480px (mobile)

---

## Responsive Breakpoints

| Breakpoint | Applies to |
|------------|------------|
| `max-width: 768px` | Tablet — nav wraps, grid becomes 2 columns |
| `max-width: 480px` | Mobile — single column layout, smaller fonts |

---

## Fonts Used

- **Bebas Neue** — headings and brand name (loaded from Google Fonts)
- **DM Sans** — body text (loaded from Google Fonts)

Both load via `<link>` in the `<head>` of each page. No internet = fonts fall back to Arial.

---

## Images

Product images are stored one folder up (`../`) from the HTML files.  
Example: `<img src="../black hoodie.jpg" alt="Black Hoodie">`

All images include `alt` text for accessibility.  
Images use `object-fit: cover` in CSS so they display consistently regardless of the original size.

---

## How to Run

Just open `index.html` in any browser. No server or installation needed.

---

## Built With

- HTML5
- CSS3 (Flexbox + CSS Grid)
- Google Fonts