# WebToolkitAI

Free, mobile-friendly online tools that help website owners create and validate AI-readable site files for SEO, GEO, and AI search visibility.

## Current Tools

- **LLMs.txt Generator**: [https://webtoolkitai.com/](https://webtoolkitai.com/)
- **LLMs.txt Validator**: [https://webtoolkitai.com/llms-txt-validator/](https://webtoolkitai.com/llms-txt-validator/)
- **AI Robots.txt Generator**: [https://webtoolkitai.com/ai-robots-txt-generator/](https://webtoolkitai.com/ai-robots-txt-generator/)

## What is This?

WebToolkitAI is a static tool site focused on AI Search / GEO / website visibility utilities. Current tools generate and validate `llms.txt` files, and generate `robots.txt` files with AI crawler policies.

## Quick Links

- **Live Site**: [https://webtoolkitai.com/](https://webtoolkitai.com/)
- **LLMs.txt Generator**: [https://webtoolkitai.com/](https://webtoolkitai.com/)
- **LLMs.txt Validator**: [https://webtoolkitai.com/llms-txt-validator/](https://webtoolkitai.com/llms-txt-validator/)
- **AI Robots.txt Generator**: [https://webtoolkitai.com/ai-robots-txt-generator/](https://webtoolkitai.com/ai-robots-txt-generator/)

## Features

- ✅ Free to use, no login required
- ✅ Mobile-first, responsive design
- ✅ No database, no API calls, no tracking
- ✅ Pure frontend — works offline after first load
- ✅ Generate, copy, and download files instantly
- ✅ Load sample data for quick testing
- ✅ Built-in crawler agent reference (13 AI agents)

## Local Development

### Option 1: Direct File Open
Simply open `index.html` in any modern browser. No build step required.

```bash
# macOS
open index.html

# Windows
start index.html

# Linux
xdg-open index.html
```

### Option 2: Local Server (Recommended for Development)

```bash
# Using Python 3
python -m http.server 8000

# Using Node.js (npx)
npx serve .

# Using PHP
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

## Deployment

### Cloudflare Pages

1. Fork or clone this repository
2. Go to Cloudflare Dashboard → Pages → Create a project
3. Connect your GitHub repository
4. Set build command to leave empty
5. Set output directory to `/` (root)
6. Deploy

### Vercel

1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in the project directory
3. Follow prompts — no build configuration needed

### Netlify

1. Drag and drop the project folder to [Netlify Drop](https://app.netlify.com/drop)
2. Or connect via GitHub for automatic deployments

### GitHub Pages

1. Push this folder to a GitHub repository
2. Go to Settings → Pages
3. Select source branch (main/root)
4. Your site will be at `https://username.github.io/repo-name/`

### Manual Upload

Upload files to any web server's root directory. That's it.

## File Structure

```
sites/llms-txt-generator/
├── index.html                        # LLMs.txt Generator (homepage)
├── llms-txt-validator/
│   └── index.html                    # LLMs.txt Validator tool
├── ai-robots-txt-generator/
│   └── index.html                    # AI Robots.txt Generator tool
├── how-to-create-llms-txt/
│   └── index.html                    # How-to guide with checklist widget
├── how-to-validate-llms-txt/
│   └── index.html                    # Validation guide with score estimator
├── llms-txt-examples/
│   └── index.html                    # Example templates with copy widget
├── robots-txt-ai-crawlers/
│   └── index.html                    # AI crawlers guide with filter table
├── block-gptbot-robots-txt/
│   └── index.html                    # Block GPTBot step-by-step guide
├── llms-txt-vs-robots-txt/
│   └── index.html                    # Comparison with decision widget
├── ai-crawler-user-agents/
│   └── index.html                    # Full agent list with search + copy
├── robots.txt
├── sitemap.xml
├── llms.txt
├── README.md
└── .gitignore
```

## What to Upload to GitHub

**Upload only the contents of this directory** (`sites/llms-txt-generator/`):

```
llms-txt-generator/
├── index.html
├── llms-txt-validator/
├── ai-robots-txt-generator/
├── how-to-create-llms-txt/
├── how-to-validate-llms-txt/
├── llms-txt-examples/
├── robots-txt-ai-crawlers/
├── block-gptbot-robots-txt/
├── llms-txt-vs-robots-txt/
├── ai-crawler-user-agents/
├── robots.txt
├── sitemap.xml
├── llms.txt
├── README.md
└── .gitignore
```

**Do NOT upload:**
- Any files from the parent project root directory
- Report files, plan files, or调研 files from the root
- The `skills/` directory
- Any other project-level files

This site is designed to be independently deployable and uploadable as a standalone repository.

## Customization

### Update Canonical URL

The canonical URL is already set to `https://webtoolkitai.com/`. If you deploy to a different domain, update these locations:

1. Each `index.html` — `<link rel="canonical" href="...">`
2. Each `index.html` — JSON-LD WebApplication `url` field

### Change Branding

All styling uses CSS custom properties (variables) at the top of each `<style>` section. Modify to match your brand:

```css
:root {
  --primary: #2563eb;
  --primary-hover: #1d4ed8;
}
```

## SEO Notes

- All pages have optimized title and meta description
- All pages have canonical URL set to `https://webtoolkitai.com/`
- JSON-LD structured data: WebApplication + FAQPage schemas on every page
- sitemap.xml includes all 10 URLs
- llms.txt describes all tools and guides

## Related Tools Roadmap

Future tools to add to this matrix:

1. **FAQ Schema Generator** — Create JSON-LD FAQ structured data
2. **Open Graph Preview Generator** — Generate and preview OG tags
3. **Sitemap.xml Generator** — Create XML sitemaps
4. **AI Content Brief Generator** — SEO content briefs from keywords
5. **Schema.org Generator** — Create JSON-LD structured data for any page type

## Disclaimer

All tools and the `llms.txt` format are experimental, community-driven projects. There is no official standard. Results may vary. Do not rely on `llms.txt` or robots.txt policies as guarantees of AI visibility, ranking, or security.

## License

MIT License — use freely for any purpose, including commercial projects.
