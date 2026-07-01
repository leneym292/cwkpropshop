# CWK Prop Shop & Events Website

This version uses GitHub Pages for free hosting and Firebase Realtime Database for customer reviews.

## Files to upload to GitHub
- `index.html`
- `CNAME` after you replace `www.yourdomain.com` with your real domain, or delete it until you buy a domain

## Firebase Realtime Database rules
Copy the contents of `database.rules.json` into Firebase > Realtime Database > Rules, then Publish.

## Review approval
New reviews save with `approved: false`.
To approve one, open Firebase > Realtime Database > Data > reviews, click the review, and change `approved` from `false` to `true`.
Approved reviews automatically appear on the website.


Update: Added a Graduations category and graduation party image gallery using local image files in assets/graduations/.
