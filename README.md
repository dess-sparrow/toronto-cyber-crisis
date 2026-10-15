# Toronto: Under Attack — Cyber Crisis Simulator

A static, client-side educational simulation inspired by the ODTN Toronto, December 2025 scenario.

## Run locally
Open `index.html` in a modern browser. No build step, packages, API keys, database, or backend are required.

## Deploy publicly
### GitHub Pages
1. Create a new public GitHub repository.
2. Upload `index.html` and this README.
3. Open **Settings → Pages**.
4. Under build/deployment, select **Deploy from a branch**, choose `main` and `/ (root)`, then save.
5. Wait for the Pages URL to appear in Settings → Pages.

### Netlify
Drag the folder containing `index.html` into Netlify's manual deploy flow, or connect the repository.

## Security design
- No backend, authentication, cookies, analytics, external scripts, or third-party libraries.
- No API keys or secrets.
- User text is processed locally; it is inserted into the page using `textContent`, not `innerHTML`.
- Input length is limited to 500 characters.
- This is a training simulation, not an operational system or an official ODTN site.

## Before submission
- Publish and verify the public URL.
- Test all four views, decision choices, reset, and public statement checker.
- Inspect the browser console and test mobile layout.
- If using a custom domain, enable HTTPS.
- Consider adding security headers at the hosting layer (e.g. a restrictive Content-Security-Policy, `X-Content-Type-Options: nosniff`, and `Referrer-Policy: no-referrer`). Validate the policy against the final hosting setup.
- Include the public hosted URL in your submission. The files in this package are not hosted automatically.
