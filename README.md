## 📘 Mini Guide: Responsive Layout with Container and Media Queries

### 🚀 Overview

This project demonstrates a simple, clean responsive web layout.
It uses a `.container` to keep content centered and restricted on large screens, combined with essential media queries to make it look great on tablets and mobile devices.

---

### 🗂 Container example

```css
.container {
  width: 100%;
  max-width: 1140px;
  margin: 0 auto;
  padding: 0 15px;
}
```

✅ This ensures your content is not too wide on big screens, and has some padding on small screens so text doesn't touch the edges.

---

### 📱 Popular breakpoints

These are the most common media query breakpoints used for general responsive websites.

```css
/* Default (very large screens) */
.container {
  width: 100%;
  max-width: 1320px;
  margin: 0 auto;
  padding: 0 15px;
}

/* Extra large devices (desktops) */
@media (max-width: 1999px) {
  .container {
    max-width: 1140px;
  }
}

/* Large devices (tablets, small laptops) */
@media (max-width: 991px) {
  .container {
    max-width: 960px;
  }
}

/* Medium devices (landscape phones, small tablets) */
@media (max-width: 767px) {
  .container {
    max-width: 720px;
  }
}

/* Small devices (portrait phones) */
@media (max-width: 575px) {
  .container {
    max-width: 100%;
    padding: 0 15px;
  }
}

```

✅ You typically start **mobile-first**, writing styles for mobile by default, and use these media queries to adjust layout for wider screens.

---

### ✨ Quick example

```css
body {
  font-size: 16px;
}

@media (max-width: 768px) {
  body {
    font-size: 14px;
  }
}

@media (max-width: 576px) {
  body {
    font-size: 13px;
  }
}
```

---

### 🏗 Recommended structure

```html
<body>
  <header>...</header>
  <div class="container">
    <main>...</main>
  </div>
  <footer>...</footer>
</body>
```

✅ Use `.container` for main content.
Let headers, footers, or full-width banners extend across the entire screen.

---

### 🚀 Run locally

```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
open index.html
```

---

## ✅ TL;DR

* Use a `.container` to **restrict content width** on large screens.
* Use **media queries** to adjust layout and font sizes for tablets & mobiles.
* Start with **mobile-first CSS**, then add `min-width` or `max-width` breakpoints for larger screens.

---
