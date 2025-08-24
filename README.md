# CheckArle — Travel Budget Calculator

A minimal, fast static site that estimates trip budgets in INR with a few inputs.

## Quick start

1. **Create a GitHub repo** (e.g., `checkarle-site`) and push these files.
2. **Default branch** should be `main`.
3. **Enable Pages**: Settings → Pages → Build from GitHub Actions.
4. (Optional) Add a `CNAME` file containing `checkarle.com` for a custom domain on GitHub Pages.

### Custom domain on GoDaddy → GitHub Pages
- In this repo, create a file named `CNAME` with only:
  ```
  checkarle.com
  ```
- In **GoDaddy DNS**, set:
  - `A` @ → `185.199.108.153`
  - `A` @ → `185.199.109.153`
  - `A` @ → `185.199.110.153`
  - `A` @ → `185.199.111.153`
  - `CNAME` `www` → `<your_github_username>.github.io`
- Wait for DNS propagate (can take a few minutes).

### Alternatively: Vercel / Netlify
- Import the repo → Framework: **None / Static**.
- Add domain `checkarle.com` in the dashboard; follow the **GoDaddy** DNS instructions they show.

## SEO checklist
- Update `<title>` and `<meta name="description">` in `index.html`.
- Verify the domain in **Google Search Console** and submit `/sitemap.xml`.
- Keep `robots.txt` as-is (it already exposes the sitemap).
- Add **Open Graph** image at `/og-image.png` for prettier shares.
- Add **FAQ schema** and **Website schema** (already included as JSON‑LD).
- Connect **Google Analytics (GA4)** by replacing the placeholder id in `index.html`.
- For **AdSense**, apply for approval, then replace the placeholder meta with your `ca-pub-...` id and add their script tag on approved pages.

## Ads & subscriptions later
- For **AdSense**, ensure content is original and helpful (add guides like “7‑day Goa budget”, “Leh-Ladakh in ₹40k”).  
- For subscriptions, consider `/pro` page gated via Razorpay/Stripe and cookie-based access.

## Local development
Just open `index.html` in your browser (no build needed).
