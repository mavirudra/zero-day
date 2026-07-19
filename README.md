# Zero-Day 🛡️

An interactive handbook explaining zero-day vulnerabilities and modern
cybersecurity — built to be a clear, beginner-friendly entry point into
how vulnerabilities are discovered, exploited, disclosed, and patched.

## What's Inside

- **Vulnerability Lifecycle** — the full journey from discovery to patch
- **What is a Zero-Day?** — core concepts explained simply
- **Case Studies** — real-world incidents like Stuxnet
- **Linux Security** — how vulnerabilities affect Linux servers and infrastructure
- **References** — the databases, standards, and reading that back this handbook

## Tech Stack

- [Astro](https://astro.build) — static site generation
- [lucide-astro](https://lucide.dev) — icons
- Vanilla CSS (no framework)

## Project Structure

```
/
├── public/
├── src/
│   ├── components/
│   │   ├── docs/          # Sidebar navigation for the docs section
│   │   ├── hero/           # Homepage hero
│   │   ├── layout/         # Navbar, Footer
│   │   ├── learn/           # "What You'll Learn" cards
│   │   ├── Lifecycle.astro
│   │   └── LifecycleStep.astro
│   ├── layouts/
│   │   ├── BaseLayout.astro
│   │   └── DocsLayout.astro
│   ├── pages/
│   │   ├── docs/           # Handbook content pages
│   │   └── index.astro     # Homepage
│   └── styles/
│       └── global.css
└── package.json
```

## Running Locally

```sh
npm install
npm run dev        # http://localhost:4321
```

| Command           | Action                                       |
| ------------------ | --------------------------------------------- |
| `npm install`       | Install dependencies                           |
| `npm run dev`       | Start local dev server at `localhost:4321`     |
| `npm run build`     | Build for production to `./dist/`              |
| `npm run preview`   | Preview the production build locally           |

## Deployment

This repo is configured to deploy automatically to GitHub Pages at
`https://mavirudra.github.io/zero-day` via GitHub Actions on every push
to `main` (see `.github/workflows/deploy.yml`).

One-time setup after pushing: in the repo, go to **Settings → Pages** and
set **Source** to **GitHub Actions**. The first push to `main` will
trigger the build and deploy automatically.

## Roadmap

- [ ] Add more case studies (Pegasus, Log4Shell, etc.)
- [ ] Expand Linux Security section with hands-on hardening examples
- [ ] Mobile nav for the docs sidebar

## Contributing

This is primarily a personal/educational project, but issues and PRs
with corrections or additional case studies are welcome.

## License

MIT
