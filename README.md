# STARHAVEN — Spaceship Renovation

A fictional premium interstellar spaceship renovation service, built as a static website and served by a Cloudflare Worker.

## Project structure

```text
.
├── public/
│   ├── index.html
│   ├── styles.css
│   ├── 404.html
│   ├── about/index.html
│   ├── services/index.html
│   └── contact/index.html
├── src/index.js
└── wrangler.toml
```

## Pages

| Path | Page |
| --- | --- |
| `/` | Starhaven homepage |
| `/services/` | Spaceship renovation services |
| `/about/` | Company story and values |
| `/contact/` | Contact details and demo enquiry form |
| Unknown paths | Custom 404 page |

## Run locally

Install Wrangler:

```bash
npm install --save-dev wrangler
```

Start the local development server:

```bash
npx wrangler dev
```

## Deploy

```bash
npx wrangler login
npx wrangler deploy
```

## Notes

- The business, prices, contact details and customer metrics are fictional demonstration content.
- The contact form uses a `mailto:` action. It does not store or transmit submissions to a backend.
- Spacecraft visuals are remotely hosted illustrative images; check the relevant source and licence before using them in a real commercial deployment.
- The site uses Google Fonts and remotely hosted images, so those assets require an internet connection.
