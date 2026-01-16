# Agentify Link Checking Test Pages

Simple standalone HTML test pages for link validation testing.

## Quick Start

### Local Testing

```bash
# Python 3
python3 -m http.server 3000

# Or Node.js (if you have npx)
npx http-server -p 3000

# Or PHP
php -S localhost:3000
```

Then visit: http://localhost:3000/

## Deployment Options

### Vercel
1. Connect this repository to Vercel
2. No build command needed
3. Deploy - files will be served as static HTML

### Netlify
1. Connect this repository to Netlify
2. No build command needed
3. Deploy - files will be served as static HTML

### GitHub Pages
1. Push to GitHub
2. Go to Settings > Pages
3. Set source to root directory
4. Deploy

### Any Static Hosting
Just upload all HTML files to your static hosting provider.

## Test Pages

- `index.html` - Index page with links to all tests
- `01-clean.html` - Clean page (control)
- `02-no-external.html` - No external links
- `03-single-bot-blocker.html` - Single bot-blocker
- `04-multiple-bot-blockers.html` - Multiple bot-blockers
- `05-bot-blocker-plus-valid.html` - Bot-blocker + valid link
- `06-broken-links.html` - Broken links only
- `07-broken-plus-bot-blocker.html` - Broken + bot-blocker
- `08-non-http-only.html` - Non-HTTP only
- `09-mixed-skipped.html` - Mixed skipped + bot-blocker
- `10-subdomain-test.html` - Subdomain normalization
- `11-redirects.html` - Redirects (301/302/307/308)
- `12-client-errors.html` - Client errors (4xx)
- `13-server-errors.html` - Server errors (5xx)
- `14-timeouts.html` - Timeouts
- `15-invalid-and-weird-urls.html` - Invalid and weird URLs
- `16-duplicate-links.html` - Duplicate links
- `17-images-mixed.html` - Images mixed
- `18-bot-protection.html` - Bot protection

## URLs

After deployment, access pages at:
- `https://yourdomain.com/` or `https://yourdomain.com/index.html`
- `https://yourdomain.com/01-clean.html`
- `https://yourdomain.com/02-no-external.html`
- etc.
