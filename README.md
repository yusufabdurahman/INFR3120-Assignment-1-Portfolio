# Yusuf Abdurahman - Personal Portfolio

# Yusuf Abdurahman - Personal Portfolio

- **Course assignment:** HTML5 and CSS3 portfolio (Fall 2026, Assignment 1)
- **Student:** Yusuf Abdurahman
- **Live site:** https://yusufabdurahman.github.io/INFR3120-Assignment-1-Portfolio/
- **Repository:** https://github.com/yusufabdurahman/INFR3120-Assignment-1-Portfolio

## About this project
A four-page personal portfolio built with HTML5 and CSS3 and hosted on GitHub Pages. It introduces me, my studies in Information Technology at Ontario Tech University, my projects and a way to contact me. The design uses a black background, blue accents and a monospace font to suit my interest in networking and cybersecurity.

## Pages
| File | Purpose |
|------|---------|
| `index.html` | Home: photo, introduction and what I work on |
| `about.html` | About Me: my story, an introduction video (controls and poster) and my interests outside school |
| `projects.html` | Projects: five projects from my courses |
| `contact.html` | Contact Me: form with HTML5 validation (name, email, cell number, comments) |

## Folder structure
| Folder | Contents |
|--------|----------|
| `css/` | `style.css` (shared styles), `mobile.css`, `tablet.css`, `laptop.css` |
| `images/` | My photo and the video poster image |
| `videos/` | `intro.mp4`, my 45-second introduction |

## Responsive design (fluid design and media queries)
The layout is fluid: widths are percentages and elements are placed with floats and inline-block. **Flexbox is not used anywhere.** `style.css` holds the shared look, and one extra stylesheet is loaded per screen size using the `media` attribute on each `<link>`.

| File | Screen width | Layout | Why these sizes |
|------|--------------|--------|-----------------|
| `mobile.css` | 320px - 767px | One column, centered | 320px is the smallest common phone width. 767px is just below a portrait tablet. |
| `tablet.css` | 768px - 1023px | Two columns (photo and text side by side, 2 cards per row) | 768px is the standard portrait tablet width. 1023px stops just before laptops. |
| `laptop.css` | 1024px and up | Three columns (3 cards per row) | 1024px is the common smallest laptop width. Content is capped at 1100px so lines stay readable. |

## Gradients
- **Linear gradient (left to right):** the header background, black to blue (`.site-header` in `style.css`).
- **Angled linear gradient (135deg):** the Home page hero background, black to dark blue (`.hero`).
- **Angled linear gradient (90deg):** the underline bar under every section heading (`.section-title::after`).
- **Angled linear gradient (160deg):** the footer, black to blue (`.site-footer`).

## Color scheme
Created with Adobe Color: EDIT: paste your Adobe Color palette link here.

| Color | Hex | Used for |
|-------|-----|----------|
| Black | `#000000` | Page background, header and footer gradients |
| Dark grey | `#141414` | Cards and alternate sections |
| Blue | `#1E6FD9` | Buttons, borders, gradients |
| Light blue | `#4DA3FF` | Links, highlights, typed role text |
| White | `#FFFFFF` | Headings and text on dark backgrounds |

White text on black and on the blue gives strong contrast. Form error messages use a lighter red (`#FF6B6B`) so they stay readable.

## Font
Courier New, a system font that is available on most computers, with Courier and the generic monospace font as fallbacks.

## Design features
- Dotted grid background, like a network diagram
- Terminal-style prompts (`$` and `>`) before headings
- Pulsing status dot beside my name in the header
- Photo with a glowing ring
- Hover effects on cards and buttons

All of these are done in CSS only.

## Contact form validation
The form uses HTML5 validation only: `required`, `type="email"`, `type="tel"` with a `pattern` for a 10-digit number, and `minlength` and `maxlength`. The browser shows a message if a field is empty or wrong. No JavaScript is used.

## Accessibility
- Semantic tags: `header`, `nav`, `main`, `section`, `article`, `figure` and `footer`
- Descriptive `alt` text on images
- A `lang` attribute and a viewport meta tag on every page
- Labels connected to every form field
- Sufficient color contrast

## Testing
| Check | Tool | Result |
|-------|------|--------|
| HTML validation | W3C Markup Validator | EDIT: add result |
| CSS validation | W3C CSS Validator | EDIT: add result |
| Links | W3C Link Checker | EDIT: add result |
| Spelling | EDIT: name your tool | EDIT: add result |
| Accessibility | WAVE | EDIT: add result |
| Screen sizes | Browser developer tools at 375px, 800px and 1280px | All pages checked |

## Credits and sources
- The layout idea (header, round photo, introduction text) was inspired by a YouTube portfolio tutorial. EDIT: add the video title and link.
- The photo and the introduction video are my own.
- Courier New is a system font, so no download or credit is needed.
- EDIT: list any other code, images or ideas you used and where they came from.
- **AI assistance:** EDIT: follow your course's policy. If AI tools were allowed, write something like "I used Claude (Anthropic) to help plan, write and debug parts of the HTML and CSS. I reviewed the code and can explain how it works."
