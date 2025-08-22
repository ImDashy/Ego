# Publish this site with GitHub Pages

1. Create a new GitHub repository (public is fine).
2. Commit and push these files to the `main` branch of your repo.
   - Ensure the `gh-pages/.github/workflows/pages.yml` remains intact.
3. In GitHub:
   - Go to Settings → Pages.
   - Set Source to "GitHub Actions" (the provided workflow will deploy automatically on push to `main`).
4. After the workflow finishes, your site will be live at:
   - https://<your-username>.github.io/<your-repo>/

Notes:
- The workflow uploads the `gh-pages` directory as the site artifact.
- If your default branch is not `main`, update the workflow trigger.