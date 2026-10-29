# Inés Pastor-Marazuela — Personal Website

Source code for my personal website, hosted at **[inespm.github.io](https://inespm.github.io/)** and built using [Astro](https://astro.build/), based on the [Astrofy](https://github.com/manuelernestog/astrofy) template.

The website combines my academic portfolio as an astrophysicist with a separate space dedicated to my crochet and knitting projects, **Craftinés PM**.

## Website structure

### Astronomy — [inespm.github.io](https://inespm.github.io/)

My academic website includes:

- **Research:** My work on fast radio bursts (FRBs), neutron stars, and radio transients.
- **Publications:** Scientific papers, with links to the published articles.
- **CV:** Education, research experience, and academic activities.
- **Outreach:** Public talks, interviews, science communication, and media appearances.
- **Gallery:** Photographs of radio telescopes, conferences, and research-related activities.
- **Contact:** Information for getting in touch.

### Craftinés PM — [inespm.github.io/crafts](https://inespm.github.io/crafts/)

A separate section dedicated to my knitting and crochet projects, featuring original designs, photographs, and patterns.

Craftinés PM uses its own visual identity and layout, independently of the academic website.

## Technologies

The website uses:

- [Astro](https://astro.build/) — Static site framework
- [Tailwind CSS](https://tailwindcss.com/) — Styling and responsive layouts
- [DaisyUI](https://daisyui.com/) — UI components
- [pnpm](https://pnpm.io/) — Package management
- [GitHub Pages](https://pages.github.com/) — Hosting
- [GitHub Actions](https://github.com/features/actions) — Automated deployment

The website is static and does not require a backend server.

## Project structure

```text
src/
├── components/         # Reusable website components
│   ├── crafts/          # Craftinés-specific components
│   └── sections/        # Academic website sections
├── layouts/
│   ├── BaseLayout.astro
│   └── CraftsLayout.astro
├── pages/
│   ├── index.astro      # Academic homepage
│   ├── publications.astro
│   ├── outreach.astro
│   ├── gallery.astro
│   ├── cv.astro
│   ├── contact.astro
│   └── crafts/          # Craftinés pages
├── styles/
└── config.ts

public/
├── crafts/              # Craftinés images and assets
├── gallery/             # Gallery photographs
├── outreach/            # Outreach images and videos
└── publications/        # Publication figures

.github/
└── workflows/
    └── deploy.yml       # GitHub Pages deployment
```

## Running locally

Clone the repository:

```bash
git clone https://github.com/InesPM/InesPM.github.io.git
cd InesPM.github.io
```

Install dependencies:

```bash
pnpm install
```

Start the local development server:

```bash
pnpm dev
```

Open [http://localhost:4321](http://localhost:4321) to preview the website.

To generate the production build:

```bash
pnpm build
```

The generated files are saved in `dist/`.

## Deployment

The website is automatically deployed to GitHub Pages using GitHub Actions.

Changes pushed to the `main` branch trigger the deployment workflow:

```bash
git add .
git commit -m "Update website"
git push origin main
```

The workflow builds the Astro website and publishes the generated static files.

## Credits

The original website structure is based on [Astrofy](https://github.com/manuelernestog/astrofy), created by [Manuel Ernesto](https://github.com/manuelernestog).

The website has been customized with new layouts, components, styling, and content.

## Contact

For academic enquiries, collaborations, or science communication opportunities, please visit the [contact page](https://inespm.github.io/contact).

For crochet and knitting projects, visit [Craftinés PM](https://inespm.github.io/crafts/).

---

© Inés Pastor-Marazuela. Website content, photographs, and original designs are my own unless otherwise credited.