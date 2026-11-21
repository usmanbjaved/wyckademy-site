# Webby · wyckademy.com

Webby is the Wyckademy agent that builds and maintains the website at **wyckademy.com**.

- **Site:** built by Webby in the Wyckoff repo (`webby/site/`, from website design v1) and copied here by
  `python webby/webby.py publish`. Pages: `/`, `/basics/`, `/lesson/`, `/trades/`, `/trades/hal-2026-11-13/`.
  Hand-kept here (Webby never touches them): `CNAME`, `privacy/`, `terms/`, `tiktok/` (Harry's TikTok sign-in page).
- **Hosting:** GitHub Pages from this repo, branch `main`, folder `/`. `CNAME` holds the custom domain.
- **Domain:** wyckademy.com, registered at GoDaddy. DNS: four A records for `@` (185.199.108.153,
  .109.153, .110.153, .111.153) and `www` CNAME to `usmanbjaved.github.io`. Microsoft 365 email records
  in GoDaddy must stay as they are.
- **Updating:** change the design or `webby.py` in the Wyckoff repo; the "Webby - build site" workflow rebuilds and
  pushes here (needs the `WEBBY_SITE_TOKEN` secret), and GitHub Pages republishes within a minute or two.
