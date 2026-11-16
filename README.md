# Basic Website Worker

A minimal Cloudflare Worker that serves a handful of static HTML pages using Cloudflare Workers Static Assets. No framework or build step is required.

## Project structure

```text
.
├── public/
│   ├── index.html
│   ├── 404.html
│   ├── about/
│   │   └── index.html
│   └── contact/
│       └── index.html
├── src/
│   └── index.js
└── wrangler.toml
```

## Requirements

- Node.js and npm
- A Cloudflare account

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

Log in to Cloudflare:

```bash
npx wrangler login
```

Deploy the Worker and its static assets:

```bash
npx wrangler deploy
```

## Pages

| Path | Page |
| --- | --- |
| `/` | Home |
| `/about/` | About |
| `/contact/` | Contact |
| Unknown paths | Custom 404 page |

## Add another page

Create a folder under `public` and add an `index.html` file. For example, `public/services/index.html` is available at `/services/`.

Static files such as CSS, JavaScript, images, and fonts can also be placed in `public` and referenced by the HTML pages.
