# 🏥 MedCare Hospital — Sign In Page

A clean, production-grade hospital web portal sign-in page built with pure HTML, CSS, and vanilla JavaScript. Features a refined clinical-luxury aesthetic with smooth animations and a fully responsive layout.

---

## 📁 Project Structure

```
hospital-signin/
├── hospital-signin.html   # Markup, structure, and JS logic
├── hospital-signin.css    # All styles, variables, and animations
└── README.md              # Project documentation
```

---

## ✨ Features

- **Split-panel layout** — branded left panel with hospital stats and a focused sign-in form on the right
- **Role-based tabs** — switch between Patient, Staff, and Admin login modes
- **Password toggle** — show/hide password with animated eye icon
- **Form validation** — inline error messaging for missing fields
- **Loading state** — spinner animation on sign-in submission
- **Hospital SSO** — single sign-on button with redirect feedback
- **Responsive design** — left panel collapses gracefully on mobile/tablet (< 900px)
- **Staggered animations** — smooth `fadeUp` entrance for each UI element on load
- **No dependencies** — zero frameworks, zero build tools required

---

## 🎨 Design System

| Token           | Value       | Usage                          |
|-----------------|-------------|--------------------------------|
| `--navy`        | `#0b1f3a`   | Primary background, buttons    |
| `--teal`        | `#1a7a6e`   | Labels, links, accents         |
| `--teal-light`  | `#22a394`   | Focus states, hover effects    |
| `--gold`        | `#c9a96e`   | Italic highlight in hero text  |
| `--cream`       | `#f7f4ef`   | Page background                |
| `--warm-white`  | `#fdfcfa`   | Right panel, input backgrounds |

**Fonts** (loaded via Google Fonts):
- `Cormorant Garamond` — headings and display text
- `DM Sans` — body, labels, buttons

---

## 🚀 Getting Started

No installation or build step required. Just clone and open.

```bash
git clone https://github.com/your-username/hospital-signin.git
cd hospital-signin
```

Then open `hospital-signin.html` in your browser:

```bash
# macOS
open hospital-signin.html

# Windows
start hospital-signin.html

# Linux
xdg-open hospital-signin.html
```

> **Note:** An internet connection is required on first load to fetch Google Fonts. The page will still function without it, falling back to system serif and sans-serif fonts.

---

## 🖥️ Browser Support

| Browser        | Support |
|----------------|---------|
| Chrome 90+     | ✅      |
| Firefox 88+    | ✅      |
| Safari 14+     | ✅      |
| Edge 90+       | ✅      |
| IE 11          | ❌      |

---

## 📐 Responsive Breakpoints

| Breakpoint   | Behavior                                      |
|--------------|-----------------------------------------------|
| `> 900px`    | Full split-panel layout (left + right panels) |
| `≤ 900px`    | Left panel hidden, right panel full width     |

---

## 🔧 Customization

All colors are defined as CSS custom properties in `:root` inside `hospital-signin.css`. To rebrand, simply update the variable values at the top of the file:

```css
:root {
  --navy:       #0b1f3a;
  --teal:       #1a7a6e;
  --teal-light: #22a394;
  --gold:       #c9a96e;
  /* ... */
}
```

To add more role tabs, add a new button inside `.role-tabs` in the HTML and update the `placeholders` object in the `setRole()` JavaScript function.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
