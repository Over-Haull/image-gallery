source:
https://codehelp-image-gallery.netlify.app/

---

# Design Specs: My Gallery

## 🎨 Color Palette

| Usage | Color | HEX/CSS Value |
| :---------------------- | :-------------------- | :------------------ |
| **Background** | Light Grey | `#f4f4f4` |
| **Heading Text** | Dark Grey | `rgb(51, 51, 51)` / `#333333` |
| **Figcaption Text** | White | `#fff` |
| **Figcaption Hover Text** | Dark Blue | `darkblue` |
| **Figcaption Gradient Start** | Black (20% Opacity) | `rgba(0, 0, 0, 0.2)` |
| **Figcaption Gradient End** | White (0% Opacity) | `rgba(255, 255, 255, 0)` |
| **Hover Drop Shadow** | Dark Grey | `#333` |

---

## ✒️ Typography

* **Global Font Family:** `'Poppins', sans-serif`

| Element | Font Size | Font Weight | Other Styles |
| :------------------------------ | :-------- | :---------- | :----------- |
| **Main Heading (`h1`)** | `40px` | `normal` | Center-aligned |
| **Figcaption (`figcaption`)** | `20px` | `700` | Center-aligned |

---

## 📏 Layout & Spacing

| Element | Property | Value |
| :-------------------------- | :-------------------------- | :------------------ |
| **Main Wrapper (`.wrapper`)**| `max-width` / `margin` / `padding` | `1200px` / `0 auto` / `20px` |
| **Main Heading (`h1`)** | `margin` | `20px auto` |
| **Container (`.container`)**| `display` / `justify-content` / `flex-wrap` | `flex` / `space-between` / `wrap` |
| **Card (`.card`)** | `width` / `height` / `margin-bottom` | `32%` / `auto` / `20px` |
| **Figcaption (`figcaption`)**| `height` / `padding` | `16%` / `25px` |

---

## ✨ Effects & Components

### Gallery Cards (`.card`)

* **Border Radius:** `10px`
* **Default Image State:** `100%` grayscale.
* **Default Figcaption State:** `opacity: 0`, `bottom: 0`.
* **Hover State:**
    * `transform: scale(1.03)` (scales up slightly).
    * `filter: drop-shadow(0 0 10px #333)` (adds a shadow).
    * **Image Hover:** `filter: grayscale(0)` (colorizes the image).
    * **Figcaption Hover:**
        * `opacity: 1` (becomes visible).
        * `bottom: 40%`.
        * `transform: translateY(-50%) rotate(360deg)` (moves up, rotates 360 degrees).
        * `color: darkblue`
* **Transitions:**
    * `card` element: `0.5s` for `transform` and `filter`.
    * `card img`: `0.5s` for `filter`.
    * `figcaption`: `1s` for `transform`, `opacity`, and `bottom`.

### Figcaption (`figcaption`)

* **Background:** `linear-gradient` from `rgba(0, 0, 0, 0.2)` to `rgba(255, 255, 255, 0)`.
* **Positioning:** `position: absolute; bottom: 0;`

---

## 🖼️ Asset List

* `favicon.ico` (located in `./img/` relative to `styles.css`)
* `image1.jpg` through `image15.jpg`/`jpeg` (located in `./img/` relative to `styles.css`)

---