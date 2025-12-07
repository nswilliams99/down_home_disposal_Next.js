# Down Home Disposal - Next.js Website

A responsive 3-page website for Down Home Disposal residential trash collection service in Middle Tennessee.

## Tech Stack

- **Framework**: Next.js 15.0.5+ (App Router) - patched for CVE-2025-55182
- **UI**: React 19, Tailwind CSS, shadcn/ui components
- **Analytics**: Google Analytics 4 (G-13N50DM7E2) + Google Tag Manager (GTM-WXD599HF)
- **SEO**: Next.js Metadata API, JSON-LD structured data, sitemap, robots.txt

## Pages

- `/` - Home page with hero, features, FAQ, and CTAs
- `/service-areas` - Pickup schedule and service area information
- `/privacy` - Privacy policy, terms of service, SMS terms

## Deploying to Vercel

### Option 1: Deploy from Subdirectory

If deploying from this repository where Next.js is in the `nextjs-app` folder:

1. Go to your Vercel project settings
2. Navigate to **Settings > General > Root Directory**
3. Set the root directory to `nextjs-app`
4. Redeploy

### Option 2: Move to Root (Recommended)

For cleaner deployment, move all Next.js files to the repository root:

```bash
# From repository root
mv nextjs-app/* .
rm -rf nextjs-app
git add .
git commit -m "Move Next.js to root"
git push
```

## Local Development

```bash
npm install
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view the site.

## Environment Variables

No environment variables required for basic operation. GA4/GTM tracking IDs are hardcoded.

## SEO Features

- Metadata API for page titles, descriptions, and Open Graph
- JSON-LD LocalBusiness schema for Google
- Automatic sitemap generation at `/sitemap.xml`
- robots.txt for search engine crawling
- Canonical URLs on all pages

## Dark Mode

Uses `next-themes` with class-based dark mode. Default is light mode.
