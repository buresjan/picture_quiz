# Picture Quiz

Static HTML picture quiz for studying visual material from the course notes.

## Run Locally

Open `public/index.html` in a browser. No build step or server is required.

## Deploy To Cloudflare Pages

For Cloudflare Pages, use these settings:

- Framework preset: `None`
- Build command: leave empty
- Build output directory: `public`

If you use Cloudflare's `npx wrangler deploy` deploy command instead, keep the
included `wrangler.jsonc`. It points Wrangler at `./public` so it does not try
to upload the repository's `.git` directory as an asset.

The app is fully static and stores the local score in the browser's `localStorage`.
