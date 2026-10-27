# austincofran.com

Personal site for Austin Cofran, photographer. Plain HTML, no build step.

- `index.html`: the whole site (styles and script inline). Bentempo look: dark sections for the work, light sections for reading and booking.
- `assets/photos/<section>/`: web-ready photos (900px and 1800px WebP)
- `assets/share.jpg`: the preview image that shows when the link is texted or posted

Testing phase:
- `<meta name="robots" content="noindex">` keeps the test link out of Google. Remove it at launch.
- `og:image` points at the workers.dev test URL. Switch it to https://austincofran.com at launch.
- The booking form isn't connected yet (needs a form service such as Formspree).

Deploy: Cloudflare (Workers static assets), connected to this repo. Every push to `main` redeploys.
