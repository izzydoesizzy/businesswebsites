# Business Websites

> AstroWind-based business website template for building high-performance marketing sites, landing pages, and professional portfolios.

![Astro](https://img.shields.io/badge/Astro-5.0-FF5D01?logo=astro&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3-06B6D4?logo=tailwindcss&logoColor=white)
![MDX](https://img.shields.io/badge/MDX-Supported-FCB32D?logo=mdx&logoColor=black)

## Overview

Business Websites is a customized AstroWind-based template designed for building high-performance business marketing sites. Built on Astro 5.0 with Tailwind CSS, it provides a comprehensive set of pre-built page templates spanning startup sites, SaaS marketing, personal portfolios, and multiple landing page variants (lead generation, click-through, pre-launch, product, sales, subscription). The template includes a full blog system with MDX support, SEO optimization, RSS feeds, and production-ready Lighthouse scores.

## Features

- **Multiple Page Templates** -- Pre-built pages for diverse business needs:
  - Home page with hero, features, steps, FAQ, stats, and CTA widgets
  - Services page
  - Pricing page
  - Contact page
  - About page
- **Industry-Specific Layouts** -- Dedicated templates under `/homes/`:
  - Startup
  - SaaS
  - Personal portfolio
  - Mobile app
- **Landing Page Variants** -- Six landing page templates under `/landing/`:
  - Lead generation
  - Click-through
  - Pre-launch
  - Product
  - Sales
  - Subscription
- **Blog System** -- MDX-powered blog with categories, tags, social sharing, and automatic RSS feed generation
- **Widget Library** -- Reusable Astro components including Hero, Features, Steps, Content, FAQs, Stats, CallToAction, BlogLatestPosts, and more
- **SEO & Performance** -- Built-in sitemap generation, Open Graph tags, analytics integration (Google Analytics, Splitbee), and image optimization via Astro Assets and Unpic
- **Dark Mode** -- Full dark mode support with Tailwind CSS
- **Responsive Design** -- Mobile-first responsive layout across all pages

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Framework | Astro 5.0 |
| Language | TypeScript 5 |
| Styling | Tailwind CSS 3 + Typography plugin |
| Content | MDX |
| SEO | @astrolib/seo, @astrojs/sitemap |
| Analytics | @astrolib/analytics |
| Icons | Iconify (Tabler + Flat Color Icons) |
| Images | Unpic (Universal image CDN), Sharp |
| RSS | @astrojs/rss |
| Linting | ESLint + Prettier |

## Getting Started

```bash
# Clone the repository
git clone git@github.com:izzydoesizzy/businesswebsites.git
cd businesswebsites

# Install dependencies
npm install

# Start the development server
npm run dev
```

The site will be available at `http://localhost:4321`.

## Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start the development server |
| `npm run build` | Build for production |
| `npm run preview` | Preview the production build |
| `npm run check` | Run all checks (Astro, ESLint, Prettier) |
| `npm run fix` | Auto-fix ESLint and Prettier issues |

## Project Structure

```
src/
├── components/
│   ├── CustomStyles.astro     # Global custom styles
│   ├── Favicons.astro         # Favicon configuration
│   ├── Logo.astro             # Site logo component
│   ├── blog/                  # Blog-specific components
│   ├── common/                # Shared utility components
│   ├── ui/                    # UI primitives
│   └── widgets/               # Page section widgets (Hero, Features, FAQs, etc.)
├── pages/
│   ├── index.astro            # Home page
│   ├── about.astro            # About page
│   ├── contact.astro          # Contact page
│   ├── pricing.astro          # Pricing page
│   ├── services.astro         # Services page
│   ├── homes/                 # Industry-specific templates
│   │   ├── startup.astro
│   │   ├── saas.astro
│   │   ├── personal.astro
│   │   └── mobile-app.astro
│   ├── landing/               # Landing page variants
│   │   ├── lead-generation.astro
│   │   ├── click-through.astro
│   │   ├── pre-launch.astro
│   │   ├── product.astro
│   │   ├── sales.astro
│   │   └── subscription.astro
│   ├── [...blog]/             # Dynamic blog routes
│   ├── rss.xml.ts             # RSS feed generator
│   ├── privacy.md             # Privacy policy
│   └── terms.md               # Terms of service
├── content/                   # Blog posts and content collections
└── layouts/                   # Page layout templates
```

## Deployment

The site can be deployed to any static hosting provider. Configuration files are included for Vercel and Netlify.

```bash
# Build for production
npm run build

# Preview the build locally
npm run preview
```

Deployment configurations included:
- `vercel.json` -- Vercel deployment settings
- `netlify.toml` -- Netlify deployment settings
- `Dockerfile` + `docker-compose.yml` -- Docker deployment with Nginx

---

**Tags:** `template`, `landing-page`
**Created:** 2025-12
**Status:** Functional
**Author:** [Izzy Piyale-Sheard](https://github.com/izzydoesizzy) -- @izzydoesizzy
