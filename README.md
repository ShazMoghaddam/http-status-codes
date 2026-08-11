# HTTP Status Codes, Decoded

A searchable field guide to the three-digit codes the web sends back on every request, grouped by class with a plain-English gloss on each one. One self-contained HTML page, no build step.

**Live:** https://shazmoghaddam.github.io/http-status-codes/

## What it does

- Search every code by number, name, or meaning, with the matching text highlighted in the results
- Filter by class, with shareable per-category links (for example `.../#client` for the 4xx codes)
- A "Must-know codes" filter for the ones you actually hit day to day
- Keyboard: press `/` to jump to search, `Esc` to clear it
- Share button (uses the native share sheet, or copies the link) and Save as PDF
- Colour-coded classes and a link-preview card for social posts

## What's inside

92 codes across 7 classes:

- **1xx Informational** — the request was received, keep going
- **2xx Success** — it worked
- **3xx Redirection** — you need to go somewhere else to finish
- **4xx Client Error** — the request was wrong
- **5xx Server Error** — the server messed up
- **Proxy & CDN codes** — the nginx, AWS load balancer and Cloudflare codes you meet in the wild
- **Vendor & informal codes** — non-standard codes from Laravel, IIS, Shopify, hosts and common conventions

The official 1xx–5xx classes cover every code in the IANA registry, including the deprecated and obsoleted ones (305, 306, 510) and the provisional 104. The last two classes are non-standard codes various servers return, so they are not exhaustive by nature.

## Put it live on GitHub Pages

1. Create a new public repo named `http-status-codes`.
2. Add `index.html` (and a `preview.png` if you want a social card) to the root of the repo.
3. Go to Settings, then Pages. Under Source pick "Deploy from a branch", branch `main`, folder `/ (root)`, and Save.
4. Give it a minute, then open https://shazmoghaddam.github.io/http-status-codes/

If you name the repo something else, update the three absolute URLs near the top of `index.html` (`canonical`, `og:url`, `og:image`) so the link-preview card resolves correctly.

## Files

- `index.html` — the page
- `preview.png` — the 1200x630 card shown when the link is shared (add your own)

Made by Shaz Moghaddam.
