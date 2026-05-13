# Odey Mofokeng — Quarto Portfolio

A professional portfolio website built with [Quarto](https://quarto.org), designed to be hosted on GitHub Pages.

## 🚀 Quick Start

### Prerequisites

1. **R** (≥ 4.2.0) — [Download](https://cran.r-project.org/)
2. **RStudio** (recommended) — [Download](https://posit.co/download/rstudio-desktop/)
3. **Quarto** (≥ 1.4.0) — [Download](https://quarto.org/docs/get-started/)

### Install Quarto from R (if not already installed)

```r
install.packages("quarto")
```

### Render the Site

**Option A: From RStudio**
1. Open `odey-portfolio.Rproj` in RStudio
2. Click **Render** in the visual editor, or run:

```r
quarto::quarto_render()
```

**Option B: From Terminal**
```bash
quarto render
```

**Option C: Live Preview**
```bash
quarto preview
```

This starts a local server with hot-reload at `http://localhost:xxxx`.

### Deploy to GitHub Pages

The site outputs to the `docs/` folder. To deploy:

1. Push the entire project to your GitHub repo
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch**
4. Select `main` branch and `/docs` folder
5. Your site will be live at `https://odeymofokeng-wits.github.io/my_portfolio/`

## 📁 Project Structure

```
odey-portfolio/
├── _quarto.yml          # Main Quarto configuration
├── custom-light.scss    # Light theme overrides
├── custom-dark.scss     # Dark theme overrides
├── styles.css           # Custom CSS (animations, cards, etc.)
├── index.qmd            # Home page (hero + featured projects)
├── about.qmd            # About, skills, education, achievements
├── projects.qmd         # Full project details with file links
├── contact.qmd          # Contact information
├── odey-portfolio.Rproj # RStudio project file
├── .gitignore           # Git ignore rules
├── .Rprofile            # R startup config
└── docs/                # Generated site (output directory)
```

## ✏️ Customisation

- **Colours**: Edit CSS custom properties at the top of `styles.css`
- **Content**: Edit the `.qmd` files — they use standard Markdown + HTML
- **Navigation**: Modify the `navbar` section in `_quarto.yml`
- **Fonts**: Change the Google Fonts import in `_quarto.yml` under `include-in-header`

## 📝 Notes

- All project file links point to your GitHub repository raw URLs
- Dark mode is built-in via Quarto's theme switcher
- The site is fully responsive for mobile and tablet
- No external JavaScript frameworks required — pure Quarto + CSS
