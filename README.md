# beyondthescreen.org

Standalone static site draft for Beyond the Screen.

## Local preview

Open `index.html` directly in a browser, or serve the directory with any static file server.

## GitHub Pages deployment

The domain is managed in Cloudflare and the static site is intended to be served by GitHub Pages.

In GitHub:

1. Go to `posix4e/bts` > Settings > Pages.
2. Set Source to "Deploy from a branch".
3. Set Branch to `main` and folder to `/ (root)`.
4. Set Custom domain to `beyondthescreen.org`.
5. Enable "Enforce HTTPS" after GitHub finishes provisioning the certificate.

In Cloudflare DNS:

- Add four `A` records for `@` pointing to GitHub Pages:
  - `185.199.108.153`
  - `185.199.109.153`
  - `185.199.110.153`
  - `185.199.111.153`
- Add a `CNAME` record for `www` pointing to `posix4e.github.io`.
