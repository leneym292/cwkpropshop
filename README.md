# CWK Prop Shop & Events Website — Phase 1 + Phase 2

This package contains your updated website with a Firebase-powered review submission form.

## Files

- `index.html` — your website
- `firestore.rules` — recommended Firebase security rules
- `CNAME` — only needed after you buy a custom domain

## Phase 1: Free website hosting

1. Create a free GitHub account.
2. Create a new public repository named `cwk-prop-shop-events`.
3. Upload `index.html` to the repository.
4. Go to Settings > Pages.
5. Under Build and deployment, choose Deploy from a branch.
6. Choose `main` and `/root`, then Save.
7. Your free website will be live at:
   `https://YOUR-GITHUB-USERNAME.github.io/cwk-prop-shop-events/`

## Phase 1: Free client reviews with Firebase

1. Go to Firebase Console.
2. Create a free project.
3. Add a Web App.
4. Copy the Firebase config.
5. Open `index.html` and replace the placeholder Firebase config values.
6. Go to Firestore Database > Create database.
7. Start in production mode.
8. Create a collection named `reviews`.
9. Go to Firestore Rules and paste the contents of `firestore.rules`.
10. Publish the rules.

New client reviews submit as `approved: false`.
To show a review on the website, open that review in Firestore and change `approved` to `true`.

## Phase 2: Cheapest custom domain

Cheapest long-term option: buy the domain through Cloudflare Registrar, Porkbun, or Namecheap.

For GitHub Pages:

1. In your GitHub repository, open Settings > Pages.
2. Enter your custom domain, such as `www.cwkpropshop.com`.
3. GitHub will create/update the `CNAME` file.
4. In your domain DNS settings, add:
   - Type: CNAME
   - Name: www
   - Target: `YOUR-GITHUB-USERNAME.github.io`
5. For the root domain, either forward `cwkpropshop.com` to `www.cwkpropshop.com`, or add GitHub Pages A records.
6. Return to GitHub Pages and check Enforce HTTPS.

## Notes

The website will work for free on GitHub Pages. The only required paid item is the custom domain, usually around $10–15/year for a standard `.com`.
