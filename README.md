# Angora Landing Page

A simple static landing page for [Angora](https://github.com/LD-C-Software/angora), a self-hosted CRM/support system. Shows the logo, a one-line description, a link to the GitHub repo, and the project's contributors.

Plain HTML/CSS/JS, no framework or build step — styled with [Pico CSS](https://picocss.com) via CDN.

## Preview locally

Serve the directory with any static file server, e.g.:

```sh
python3 -m http.server 8080
```

Then open http://localhost:8080.

## Deploying to Netlify

No build command is needed — `netlify.toml` already sets the publish directory to the repo root.

**Connect the Git repo (recommended):**

1. Push this repo to GitHub.
2. In Netlify: "Add new site" → "Import an existing project" → select this repo.
3. Netlify picks up `netlify.toml` automatically — click Deploy.

**Or deploy from the CLI:**

```sh
npx netlify-cli deploy --prod
```

## Structure

- `index.html` — the whole page
- `assets/` — logo assets copied from the main Angora repo (`~/projects/angora/assets`)
- `netlify.toml` — Netlify publish config + security headers

## License

MIT, matching the main [Angora](https://github.com/LD-C-Software/angora) project.
