# tarnsoftware.co.uk

The Tarn Software website, served by GitHub Pages at https://tarnsoftware.co.uk. It is the studio's site, not
one game's: each game gets a folder and a row on the home page.

- `index.html`: home page. The hero is the logo as a tarn (sky, horizon, reflection); below it the Games list
  (one `li.game` per game) and Contact.
- `style.css`: the whole site. Colours come from the logo (night, slate, snow, glacier, moon, mist); type is
  Jost from Google Fonts.
- `assets/`: the logo files (`tarn-logo-*`, `tarn-icon-*`) and `tarn-wordmark.svg`, the logo's text on its own
  for the home hero.
- `hole-crunch/`: the Hole Crunch page (`img/` holds its icon and screenshots, 540x960 JPEGs).
- `hole-crunch/privacy/`: the Hole Crunch privacy policy. Its URL goes in the Play listing and in the game's
  `AdConfig.PublishedPrivacyPolicyUrl` (Settings and the consent prompt link to it). Do not move it, and update
  the effective date when it changes.
- `sinkhole/`: redirects to `hole-crunch/`. Sinkhole was the game's working title until 2026-10-27, and builds
  from before the rename link to `/sinkhole/privacy/`, so keep both redirect pages.
- `app-ads.txt`: authorised ad sellers; ad networks read it from the domain root (the Play listing's website
  is `https://tarnsoftware.co.uk`). The list is Unity's, from the Unity dashboard: Monetization > Settings >
  Organization > App-ads.txt. Unity changes it from time to time, so recheck monthly. Each ad network added in
  LevelPlay later brings its own lines.
- `CNAME`: the custom domain for GitHub Pages.

Adding a game: copy `hole-crunch/` to the new game's folder, swap its text, icon and screenshots, give it its own
privacy policy, and add a `li.game` row to the Games list on the home page.

DNS (GoDaddy): the apex `A` records point at GitHub Pages (185.199.108.153, 185.199.109.153,
185.199.110.153, 185.199.111.153) and `www` is a `CNAME` to `tarnsoftware.github.io`. The `MX` and other
email records belong to Microsoft 365 and must not be changed.
