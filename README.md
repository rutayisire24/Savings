# Savings Calculator

An **interactive, web‑based calculator** for visualizing the growth of regular savings over time. Built with **Quarto** and **Observable JavaScript (OJS)**, this tool produces a static HTML page that requires no server.

## Features

- **Contribution frequency**: Daily, Weekly, or Monthly
- **Custom inputs**: Amount per period, percentage of periods saved, projection horizon (1–10 years), and annual interest rate
- **Real‑time output**: Dynamic table and bar chart showing cumulative contributions and future value (in UGX)
- **Purely static**: Publish via GitHub Pages, Netlify, or any static host; no backend needed

## Getting Started

1. **Install Quarto** (https://quarto.org) and clone this repo:
   ```bash
   git clone https://github.com/<your‑username>/Savings.git
   cd Savings
   ```
2. **Render locally**:
   ```bash
   quarto preview savings_quarto.qmd --to html
   ```
3. **Open** `http://localhost:4242` in your browser to interact.

## Deployment via GitHub Pages

1. Ensure `_quarto.yml` has:
   ```yaml
   project:
     type: website
     output-dir: docs
   ```
2. Render and commit the `docs/` folder:
   ```bash
   quarto render
   git add docs
   git commit -m "Build site"
   git push
   ```
3. Add an empty `.nojekyll` in `docs/` to disable Jekyll.
4. In GitHub → Settings → Pages, select branch `main` and folder `/docs`.
5. Visit `https://<username>.github.io/Savings/` (or your custom domain).

## Custom Domain

If you own `mysite.com`, add a `docs/CNAME` file with:
```
mysite.com
```
and configure your DNS records (A‑records and CNAME) as described in the repo wiki.

## License

This project is released under the [MIT License](LICENSE).


 
