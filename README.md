[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/4tyCbCZM)
# Matope Pottery Studio

**Assignment:** ELE-IWS-521 – Internet and Web Services (Assignment 2)
**Group:** Team 3
**Theme:** Small Pottery Studio
**Breakpoint:** `640px`
**Google Font:** Playfair Display

---

## Project Structure

```text
/
├── index.html              # Clean, working version
├── style.css               # Clean styles
├── buggy-version.html      # Buggy version (Part B)
├── buggy-version.css       # Buggy styles (Part B)
├── BUILD_LOG.md            # Build log with screenshots
├── README.md               # This file
└── screenshots/            # Screenshots for Part C
```

---

##  Team Members

| Name                    | Role                    | Bug Owned                  |
| ----------------------- | ----------------------- | -------------------------- |
| **Andrea Aston**        | Navigation + Hero       | #2 – Inline `display:flex` |
| **Uchindami Mkanawire** | Feature Cards           | #5 – Missing `box-sizing`  |
| **Annie Thomas**        | Studio Section + Footer | #7 – Missing `flex-wrap`   |

---

## Features

* **Semantic HTML5** – `<nav>`, `<header>`, `<main>`, `<section>`, `<footer>`
* **Flexbox layout** – Feature cards in a row, stacking at `640px`
* **Google Font** – Playfair Display loaded from Google Fonts
* **External image** – Handmade ceramics from Unsplash
* **Responsive** – Cards stack vertically on mobile (≤ 640px)

---

## Bugs (Part B)

All bugs are planted in `buggy-version.html` and `buggy-version.css`:

| Bug #  | Owner               | Description                                                         |
| ------ | ------------------- | ------------------------------------------------------------------- |
| **#7** | Annie Thomas        | Missing `flex-wrap` → nav overflows on mobile                       |
| **#2** | Andrea Aston        | Inline `style="display:flex; flex-direction:row"` beats media query |
| **#5** | Uchindami Mkanawire | Missing `box-sizing: border-box` → padded boxes overflow            |

---

## Network Investigation (Part C)

* Google Font request: **Status 200** | Content-Type: `text/css`
* CSS blocks rendering until loaded (render-blocking)
* External image takes longer due to DNS + TCP + SSL overhead
* Font cached with `Cache-Control: max-age=...` → shows `200 (disk cache)`

---

## How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/Student-Work-Classroom-Demo-MUBAS/html-and-css-landing-page-group-three.git
   ```

2. Open `index.html` in your browser.

3. For the buggy version, open `buggy-version.html`.

---

## 📝 Live Page

View the live page here:

[Matope Pottery Studio – GitHub Pages](https://student-work-classroom-demo-mubas.github.io/html-and-css-landing-page-group-three/)



## 📄 License

This project was created for educational purposes as part of the BECE5  2026 Internet and Web Services course at MUBAS.
