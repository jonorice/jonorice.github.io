# Academic economist website template (Quarto + GitHub Pages)

This is a minimal multi page Quarto website template designed for an academic economist.

## Quick start

1. Install Quarto from https://quarto.org
2. Preview the site locally

```bash
quarto preview
```

3. Render the site to the `docs/` folder

```bash
quarto render
```

## Publishing to GitHub Pages (simple method)

This template renders to `docs/` so you can publish from your `main` branch without GitHub Actions.

1. Create a new GitHub repository (for example `my-website`)
2. Commit and push this folder to the repository
3. In GitHub, go to Settings, then Pages
4. Under Build and deployment, set Source to Deploy from a branch
5. Choose Branch `main` and Folder `/docs`
6. Save, wait for the site to deploy

Your site URL will be `https://<username>.github.io/<repository>/`

## Custom domain (optional)

Quarto recommends storing a `CNAME` file at the project root (next to `_quarto.yml`), so it is copied into the rendered site output.

Create a file called `CNAME` with one line, for example

```
www.example.com
```

Then re render, commit, and push.

You still need to configure DNS records with your domain registrar.

## Updating content

Edit the `.qmd` files and run

```bash
quarto render
```

Then commit and push your changes.
