# Kash Documentation

Public documentation for **Kash** — prediction markets on Base. This repo powers [docs.kash.bot](https://docs.kash.bot), built with [Mintlify](https://mintlify.com).

[![Website](https://img.shields.io/badge/Website-kash.bot-FBD109)](https://kash.bot)
[![Twitter](https://img.shields.io/badge/Twitter-@kash_bot-1DA1F2)](https://x.com/kash_bot)
[![Discord](https://img.shields.io/badge/Discord-Community-7289DA)](https://discord.com/invite/n9eumqjMPb)
[![Docs](https://img.shields.io/badge/Docs-Live-FBD109)](https://docs.kash.bot)

## About Kash

Kash is a prediction markets platform built on Base (Coinbase's L2). Users trade multi-outcome markets in the webapp at [app.kash.bot](https://app.kash.bot), with optional tweet-based trading via [@kash_bot](https://x.com/kash_bot) and embeddable markets for partners.

Key characteristics documented here:

- **Webapp-first**: app.kash.bot is the primary product; X integration and embeds are companion surfaces
- **Gasless**: platform-sponsored transactions via ERC-4337 account abstraction
- **Self-custodial**: a Privy-powered embedded wallet signs for the user's smart account — Kash cannot withdraw user funds; trades execute only under permissions the user authorizes
- **USDC-denominated**: trading and settlement in USDC on Base

## Repository Structure

Content is organized by the tabs in `docs.json`:

- **`getting-started/`** — user-facing docs: quick start, guides, features, ecosystem, FAQs
- **`developer-docs/`** — REST API, webhooks, CLI, SDKs, and embed API reference (parts are generated/synced from code — check before hand-editing)
- **`for-businesses/`** — B2B / white-label docs for organizations and partners (new section)
- **`assets/`** — images and other static assets
- **`docs.json`** — navigation, theming, SEO, and footer configuration

## Local Development

### Prerequisites

Node.js, plus the Mintlify CLI (optional if you use `npx`):

```bash
npm i -g mint
```

### Running the Docs

From the repo root (where `docs.json` is located):

```bash
npx mint dev
```

The documentation will be available at `http://localhost:3000`.

### Making Changes

- Edit `.mdx` files in the section directories listed above
- Update navigation in `docs.json` when adding, moving, or removing pages
- Add assets to the `assets/` directory
- Changes hot-reload in the dev server

## Deployment

Documentation is automatically deployed to [docs.kash.bot](https://docs.kash.bot) when changes are pushed to the main branch.

## Contributing

We welcome contributions to improve the documentation:

1. Fork this repository
2. Create a feature branch
3. Make your changes and preview them locally with `npx mint dev`
4. Submit a pull request

### Content Guidelines

- Use clear, concise language and practical examples
- Only document features that are live — mark planned features clearly as planned
- Follow the existing Mintlify component style (`<Note>`, `<Warning>`, `<AccordionGroup>`, `<CardGroup>`, ...)
- Keep frontmatter (`title`, `description`, `icon`) on every page
- Test all code examples

## Project Links

- **Website**: [kash.bot](https://kash.bot)
- **Documentation**: [docs.kash.bot](https://docs.kash.bot)
- **Twitter**: [@kash_bot](https://x.com/kash_bot)
- **Discord**: [Community](https://discord.com/invite/n9eumqjMPb)
- **GitHub**: [KashDAO](https://github.com/KashDAO)
- **Telegram**: [KashDAO](https://t.me/kashDAO)

## License

This documentation is open source and available under the MIT License.

---

**Kash** — Where Opinions Become Opportunities
