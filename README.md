# LLMs.txt Generator

A free, mobile-friendly online tool that helps website owners create an AI-readable `llms.txt` file for improved visibility in ChatGPT, Claude, Perplexity, Gemini, and other AI search tools.

## What is This?

LLMs.txt Generator is a standalone website tool that creates `llms.txt` files — an emerging experimental practice that helps AI systems understand your website's structure, purpose, and key content.

## Quick Links

- **Live Tool**: [https://webtoolkitai.com/](https://webtoolkitai.com/)

## Features

- ✅ Free to use, no login required
- ✅ Mobile-first, responsive design
- ✅ No database, no API calls, no tracking
- ✅ Pure frontend — works offline after first load
- ✅ Generate, copy, and download your llms.txt instantly
- ✅ Load sample data for quick testing
- ✅ Supports all optional fields (docs, blog, pricing, API docs, contact)

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

1. Drag and drop the `index.html` file to [Netlify Drop](https://app.netlify.com/drop)
2. Or connect via GitHub for automatic deployments

### GitHub Pages

1. Push this folder to a GitHub repository
2. Go to Settings → Pages
3. Select source branch (main/root)
4. Your site will be at `https://username.github.io/repo-name/llms.txt`

### Manual Upload

Upload `index.html` to any web server's root directory. That's it.

## File Structure

```
llms-txt-generator/
├── index.html      # Complete standalone website
├── README.md       # This file
└── .gitignore      # Git ignore file
```

## What to Upload to GitHub

**Upload only the contents of this directory** (`sites/llms-txt-generator/`):

```
llms-txt-generator/
├── index.html
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

The canonical URL is already set to `https://webtoolkitai.com/`. If you deploy to a different domain, update these locations in `index.html`:

1. `<link rel="canonical" href="...">`
2. JSON-LD WebApplication `@id` field

### Change Branding

All styling uses CSS custom properties (variables) at the top of the `<style>` section. Modify these to match your brand:

```css
:root {
  --color-primary: #2563eb;
  --color-primary-hover: #1d4ed8;
  /* ... */
}
```

## SEO Notes

- Title and meta description are already optimized for "LLMs.txt Generator" and related keywords
- JSON-LD structured data includes WebApplication and FAQPage schemas
- The canonical URL is set to `https://webtoolkitai.com/`
- Content includes 500+ words of explanatory text for search engines

## Related Tools

This is the first tool in a planned tool matrix. Similar tools that can be built:

1. **robots.txt Generator** — Create robots.txt files with AI crawler directives
2. **sitemap.xml Generator** — Generate XML sitemaps for search engines
3. **Schema.org Generator** — Create JSON-LD structured data for websites
4. **Open Graph Generator** — Generate OG tags for social sharing
5. **AI Content Brief Generator** — Create SEO content briefs from keywords

## Disclaimer

This tool and the `llms.txt` format are experimental, community-driven projects. There is no official standard. Results may vary. Do not rely on `llms.txt` as a replacement for proper SEO fundamentals.

## License

MIT License — use freely for any purpose, including commercial projects.
