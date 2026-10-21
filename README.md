# Kash Documentation

Public documentation for **Kash**, a social prediction market on Solana. This repo powers [docs.kash.bot](https://docs.kash.bot), built with [Mintlify](https://mintlify.com).

[![Website](https://img.shields.io/badge/Website-kash.bot-FBD109)](https://kash.bot)
[![Twitter](https://img.shields.io/badge/Twitter-@kash_bot-1DA1F2)](https://x.com/kash_bot)
[![Discord](https://img.shields.io/badge/Discord-Community-7289DA)](https://discord.com/invite/n9eumqjMPb)
[![Docs](https://img.shields.io/badge/Docs-Live-FBD109)](https://docs.kash.bot)

## About Kash

Kash is an interface built on an open, permissionless on-chain protocol on Solana that anyone can use directly. Markets on Kash are created and traded on that protocol, and Kash operates the automated market creation and resolution system. Users trade multi-outcome markets in USDC in the web app at [app.kash.bot](https://app.kash.bot) or by replying to market posts on X with [@kash_bot_trade](https://x.com/kash_bot_trade). Creators connect their X account in the web app and create markets by chatting with Kash AI.

Key characteristics documented here:

- **Web app and X**: app.kash.bot for everything, plus trading by reply on X
- **Non-custodial**: each user has their own embedded Solana wallet; Kash never holds custody of user funds, and the private key can be exported
- **No SOL needed**: Kash pays the Solana network fees
- **USDC-denominated**: trading and settlement in USDC on Solana
- **Chat-created markets**: Kash AI drafts each market; outcomes are determined by Kash's automated resolution system from published sources and rules, with a dispute window

## Repository Structure

Content is organized by the tabs in `docs.json`:

- **`getting-started/`** — user-facing docs: quick start, guides, features, ecosystem, FAQs
- **`developer-docs/`** — REST API, webhooks, CLI, SDKs, and embed API reference (parts are generated/synced from code — check before hand-editing)
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
