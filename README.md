# Personal Portfolio II — Nida Shah

**CS344: Web Engineering — Lab 3 (HTML Advanced)**
Department of Computing · Fall 2026


| **Live site** | https://nidashah612.github.io/portfolio/ |
| **Repository** | https://github.com/nidashah612/portfolio |

---

## 1. About the Project

This is a five-page personal portfolio website that extends my Lab 2 portfolio. In this lab the site was reorganised into proper folders, all styling was moved into one external stylesheet, layouts were rebuilt with CSS `float` and `clear`, and the project was published online with Git and GitHub Pages.

Only **HTML and CSS** are used. There is no JavaScript, no framework and no CSS library.

## 2. Pages

### Home — `index.html`
Introduction, role, short bio and call-to-action buttons. The profile photo floats right and the text floats left.

### Hobbies — `hobbies.html`
Four hobby cards (Reading, Photography, Coding, Traveling) floated into two columns.

### Skills — `skills.html`
Programming languages, spoken languages and other skills, shown as tag badges inside cards.

### Gallery — `gallery.html`
Image gallery with 5 photos and captions, floated three per row.

### Contact — `contact.html`
Email, phone and LinkedIn details. The profile photo floats left with the text beside it.

---

## 3. Project Structure

```
portfolio/
├── index.html
├── hobbies.html
├── skills.html
├── gallery.html
├── contact.html
├── README.md
├── css/
│   └── style.css
└── images/
    ├── profile.png
    ├── img1.jpg
    ├── img2.jpg
    ├── img3.jpg
    ├── img4.jpg
    └── img5.jpg
```

`index.html` is the home page. It has this name so that GitHub Pages opens it automatically.

## 4. Lab Requirements and How They Were Met

| Requirement | How it was done |
|---|---|
| Organise files into folders | HTML files at the root, CSS in `css/`, all images in `images/` |
| External CSS file | Every page links to `css/style.css` with `<link rel="stylesheet" href="css/style.css">`. No inline or internal CSS remains. |
| Consistent fonts, colours, borders, spacing | One dark theme with a pink accent (`#ec1561`), the Segoe UI font stack, and shared card, heading and footer styles |
| Horizontal navigation menu | Nav links are list items with `float: left`, and the Contact button uses `float: right` |
| `float` to place content side by side | Home (text and photo), Contact (photo and text), Hobbies (two columns), Gallery (three per row) |
| `clear` to fix layout issues | `.clearfix` on parent containers, `clear: left` to start each new row, and `clear: both` on the footer |
| Gallery with at least 5 images | 5 images aligned with float and clear |
| Git version control | Repository initialised, all files committed and pushed to GitHub |
| GitHub Pages deployment | Deployed from the `main` branch, `/ (root)` |

## 5. How float and clear Are Used

- **Navigation:** the logo, link list and Contact button are all floated. The `.clearfix` class on the bar stops it collapsing to zero height.
- **Home hero:** the photo is `float: right` at about 34% width and the text is `float: left` at about 58%.
- **Contact card:** the round profile photo is `float: left` so text wraps beside it. `clear: both` on the closing note moves it below the photo.
- **Hobbies:** each card is `float: left` at about 48% width. `clear: left` on every odd card starts a new row.
- **Gallery:** each item is `float: left` at 32% width. `clear: left` on every 4th item, plus the `:nth-child(3n)` margin rule, keeps rows tidy.
- **Footer:** `clear: both` keeps it below all floated content.

## 6. Run Locally

1. Download or clone the repository.
2. Open `index.html` in any modern browser (Chrome, Edge, Firefox).

```
git clone https://github.com/nidashah612/portfolio.git
```

## 7. Version Control and Deployment

```
git init
git add .
git commit -m "Lab 3: portfolio with external CSS and folders"
git branch -M main
git remote add origin https://github.com/nidashah612/portfolio.git
git push -u origin main
```

GitHub Pages: repository **Settings → Pages → Source: Deploy from a branch → `main` / `(root)` → Save**.

## 8. Tools Used

- Visual Studio Code
- Google Chrome
- Git and GitHub (GitHub Pages)

## 9. Author

**Nida Shah** — Software Engineering Student
GitHub: [nidashah612](https://github.com/nidashah612)
