# Astro Starter Kit: Blog

```sh
npm create astro@latest -- --template blog
```

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

Features:

- ✅ Minimal styling (make it your own!)
- ✅ 100/100 Lighthouse performance
- ✅ SEO-friendly with canonical URLs and Open Graph data
- ✅ Sitemap support
- ✅ RSS Feed support
- ✅ Markdown & MDX support

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
├── public/
├── src/
│   ├── components/
│   ├── content/
│   ├── layouts/
│   └── pages/
├── .github/workflows/
├── astro.config.mjs
├── wrangler.toml
├── README.md
├── package.json
└── tsconfig.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

The `src/content/` directory contains "collections" of related Markdown and MDX documents. Use `getCollection()` to retrieve posts from `src/content/blog/`, and type-check your frontmatter using an optional schema. See [Astro's Content Collections docs](https://docs.astro.build/en/guides/content-collections/) to learn more.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |
| `npx wrangler deploy`     | Deploy to Cloudflare Workers (recommended)        |

## 🚀 Deployment

### Cloudflare Workers (Recommended)

This project is configured for server-side rendering and uses Cloudflare Workers for deployment.

**Automatic Deployment**:
- Push changes to the `master` branch
- GitHub Actions will automatically build and deploy to Cloudflare Workers

**Manual Deployment**:
```bash
# Build the project
npm run build

# Deploy to Cloudflare Workers
npx wrangler deploy
```

**Prerequisites**:
1. Install Wrangler CLI: `npm install wrangler@latest --save-dev`
2. Authenticate with Cloudflare: `npx wrangler login`
3. Configure secrets in Cloudflare (if needed):
   - `npx wrangler secret put CLOUDFLARE_API_TOKEN`

## 👀 Want to learn more?

Check out [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).
