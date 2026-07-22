# CREDIT HOME — Website

Three landing-page design options for CREDIT HOME, a mobile real estate service
serving all of Florida (Central Florida focused). Static HTML — no build step, no
dependencies. Ready to host on GitHub Pages.

## Files
- `index.html` — chooser page showing all three options side by side
- `option1.html` — **Luxury Concierge** (dark + gold, serif, premium)
- `option2.html` — **Coastal Trust** (bright blue/teal, friendly, approachable)
- `option3.html` — **Bold Mobile** (dark + amber, big type, energetic)

## Preview locally
Just double-click any `.html` file to open it in your browser.

## Publish to GitHub Pages
1. Create a new repository on GitHub (e.g. `credit-home-website`).
2. Upload these files (drag them into the repo's "Add file → Upload files").
3. Go to **Settings → Pages**.
4. Under **Source**, choose **Deploy from a branch**, pick `main` and `/ (root)`, Save.
5. Your site goes live at `https://<your-username>.github.io/credit-home-website/`.

### Making your chosen design the homepage
GitHub Pages serves `index.html` by default. Once you pick a design:
- Rename the current `index.html` (chooser) to `chooser.html`, then
- Rename your chosen file (e.g. `option2.html`) to `index.html`.

### Custom domain (optional)
In **Settings → Pages → Custom domain**, enter your domain (e.g. `credithome.com`)
and add a `CNAME` DNS record at your registrar pointing to `<username>.github.io`.

## Contact form setup (2 minutes — required for the form to send)
Every page has a real contact form wired to **Web3Forms** (free, no account, works
on static hosting like GitHub Pages). To turn it on:
1. Go to **https://web3forms.com**, enter your email, and copy the **Access Key**
   they send you (a short code).
2. In each HTML file you're publishing, find this line:
   `<input type="hidden" name="access_key" value="YOUR_WEB3FORMS_ACCESS_KEY">`
3. Replace `YOUR_WEB3FORMS_ACCESS_KEY` with your key. Done — submissions now arrive
   in your email inbox.

(If you only publish one design, you only need to update that one file.)

## Images
- The site ships with **real, royalty-free stock photos** (in `images/`) — homes,
  interiors, keys, an agent portrait, Florida lifestyle, and a Sprinter van.
- **`images/van.jpg` is a stock van** — replace it with a real photo of YOUR van
  (keep the same filename and it drops straight in). Each page marks it
  "Placeholder — swap for a photo of your van".
- The **Listings & Lifestyle gallery** uses `home-*.jpg`, `interior-*.jpg`,
  `keys.jpg`, `florida-palms.jpg` — swap any of these for your own listing/past-sale
  photos (same filenames = no code changes needed).

## Before launch — also update
- **Client testimonials** — the three reviews on each page are placeholders.
- **Contact info** — the `tel:` and `mailto:` links (search for `+10000000000`
  and `hello@credithome.com`).
- **Logo** — drop your logo into the header where the "CREDIT HOME" text sits.
- **Colors / fonts** — adjustable at the top of each file's `<style>` block
  (the `:root` CSS variables).

## Notes
- Fully responsive (mobile, tablet, desktop) with a working mobile menu.
- Fonts load from Google Fonts; images are local; the form posts to Web3Forms.
  Everything else is self-contained — no build step.
