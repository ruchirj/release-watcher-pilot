# Release Watcher pilot

This synthetic fixture publishes a static page through GitHub Pages. Run **Deploy test site** on `main` to produce a GitHub deployment in the `github-pages` environment. GitHub records the successful deployment after Pages publishes the site.

Run **Exercise deployment controls** on `main` to validate filtering:

- **selected-environment-failure** fails preflight in `github-pages` before changing the live site.
- **preview-environment-success** publishes a short-lived artifact in `release-watcher-preview`.
