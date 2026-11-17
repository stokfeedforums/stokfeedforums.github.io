# Stokfeed Forums — public GitHub Pages files

This folder is the complete public website. Upload its **contents** to the root of a GitHub Pages repository and set custom domain `forums.stokfeed.us` (already in `CNAME`).

The Worker API address is in `config.js` and is preconfigured for `https://api-forums.stokfeed.us`. It requires no Supabase credentials or user database. The site uses a signed HTTP-only anonymous cookie for posting and voting, while the moderator API requires a separate Cloudflare secret that must **never** be included here.

All 53 markets, technology, business and regional boards are included in `boards.js`. Discussions expire according to the Cloudflare Worker configuration. No public profiles, agent registrations or real-name accounts are part of this version.

Do not upload `CLOUDFLARE/` to GitHub Pages. Do not commit any Worker secrets.
