# WebToolkitAI

Free, mobile-friendly online tools that help website owners create and validate AI-readable site files for SEO, GEO, and AI search visibility.

## Current Tools

- **LLMs.txt Generator**: [https://webtoolkitai.com/](https://webtoolkitai.com/)
- **LLMs.txt Validator**: [https://webtoolkitai.com/llms-txt-validator/](https://webtoolkitai.com/llms-txt-validator/)

## What is This?

WebToolkitAI is a small static tool site focused on AI Search / GEO / website visibility utilities. The first tool creates `llms.txt` files; the second validates pasted `llms.txt` content for structure, clarity, URLs, and common publishing issues.

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
├── index.html                  # LLMs.txt Generator
├── llms-txt-validator/
│   └── index.html              # LLMs.txt Validator
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

## Related Tools Roadmap

This is the first tool in a planned tool matrix. Similar tools that can be built:

1. **LLMs.txt Validator** — Check llms.txt files before publishing
2. **AI robots.txt Generator** — Create robots.txt files with AI crawler directives
3. **FAQ Schema Generator** — Create JSON-LD FAQ structured data
4. **AI Search Readiness Checker** — Review site visibility basics
5. **Open Graph Preview Generator** — Generate and preview OG tags for social sharing

## Disclaimer

This tool and the `llms.txt` format are experimental, community-driven projects. There is no official standard. Results may vary. Do not rely on `llms.txt` as a replacement for proper SEO fundamentals.

## License

MIT License — use freely for any purpose, including commercial projects.
