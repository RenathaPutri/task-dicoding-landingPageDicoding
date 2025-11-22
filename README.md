# Dicoding Indonesia Landing Page

A simple static landing page inspired by Dicoding Indonesia.  
This page showcases a hero section with a brief description, navigation menu, call-to-action button, and social media links.

## Features

- Top navigation bar with logo and menu links
- Hero section with:
  - Title and description about Dicoding Indonesia
  - Call-to-action button ("Lebih lanjut")
  - Illustration image
- Social media sidebar with Font Awesome icons:
  - YouTube
  - LinkedIn
  - Twitter
  - Facebook
- Uses semantic HTML structure (`header`, `main`, `aside`)
- Custom styling via external CSS

## Tech Stack

- **HTML5**
- **CSS3**
- **Google Fonts** – Quicksand
- **Font Awesome** – social media icons

## Project Structure

```txt
.
├── index.html
├── css/
│   └── app.css
└── img/
    ├── dicoding-header-logo.png
    └── circle-g.jpg
````

> Update file names or paths if your asset structure is slightly different.

## Getting Started

### Prerequisites

No special setup required. Any modern web browser will work.

Optional tools:

* Code editor (VS Code, etc.)
* Live Server extension (for auto-refresh while editing)

### How to Run

1. Clone the repository:

```bash
git clone https://github.com/<your-username>/<your-repo-name>.git
cd <your-repo-name>
```

2. Open `index.html` in your browser:

* Double-click `index.html`, **or**
* Use Live Server in VS Code:

  * Open the folder in VS Code
  * Right-click `index.html`
  * Choose **"Open with Live Server"**

## Page Overview

### Header (Navbar)

* Contains the Dicoding logo:

  ```html
  <img src="img/dicoding-header-logo.png" alt="Dicoding Indonesia" />
  ```

* Navigation menu with links:

  * Beranda
  * Menu
  * Apa yang Baru
  * Kontak

> Currently the links use `href="#"` as placeholders and can be updated to real sections or pages.

### Main Content

#### Hero Section

* Left side: description content

  ```html
  <h1 class="title">Dicoding Indonesia</h1>
  <p>...deskripsi tentang pendidikan teknologi dan talenta digital...</p>
  <button>Lebih lanjut</button>
  ```

* Right side: illustration image

  ```html
  <img src="img/circle-g.jpg" alt="Dicoding Indonesia" />
  ```

This section is wrapped inside:

```html
<div class="content">
  <div class="content-description">...</div>
  <div class="content-image">...</div>
</div>
```

Styling and layout (e.g. flexbox) are handled in `css/app.css`.

### Social Media Sidebar (Aside)

An `aside` element contains a vertical list of social media icons:

```html
<aside>
  <div class="social-media">
    <ul>
      <li><a href="#"><i class="fab fa-youtube"></i></a></li>
      <li><a href="#"><i class="fab fa-linkedin-in"></i></a></li>
      <li><a href="#"><i class="fab fa-twitter"></i></a></li>
      <li><a href="#"><i class="fab fa-facebook"></i></a></li>
    </ul>
  </div>
</aside>
```

Icons are loaded from **Font Awesome** CDN.

## Styling & Assets

### CSS

Custom styles are loaded from:

```html
<link rel="stylesheet" href="css/app.css" />
```

The CSS file is responsible for:

* Layout of the navbar, main content, and sidebar
* Typography using the Quicksand font
* Button appearance and hover states
* Alignment of logo, hero text, and image

### Fonts

Google Fonts – Quicksand:

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@300..700&display=swap" rel="stylesheet">
```

### Icons (Font Awesome)

Font Awesome is loaded via CDN:

```html
<link
  rel="stylesheet"
  href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css"
  integrity="sha512-1ycn6IcaQQ40/MKBW2W4Rhis/DbILU74C1vSrLJxCq57o941Ym01SwNsOMqvEBFlcgUa6xLiPY/NS5R+E6ztJQ=="
  crossorigin="anonymous"
  referrerpolicy="no-referrer"
/>
```

## Possible Improvements

* Make the layout fully responsive on mobile (e.g. stack content vertically)
* Add smooth scroll or link sections for the navbar menu
* Replace `href="#"` with real anchor targets or external links
* Add hover effects for the social media icons and button
* Add a footer with copyright or contact info
