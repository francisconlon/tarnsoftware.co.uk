# tarnsoftware.co.uk

The Tarn Software website, served by GitHub Pages at https://tarnsoftware.co.uk.

- `index.html`: home page.
- `sinkhole/privacy/`: the Sinkhole privacy policy. Its URL goes in the Play listing and in the game's
  `AdConfig.privacyPolicyUrl` (the consent prompt links to it). Update the effective date when it changes.
- `app-ads.txt`: authorised ad sellers; ad networks read it from the domain root. Paste LevelPlay's lines in.
- `CNAME`: the custom domain for GitHub Pages.

DNS (GoDaddy): the apex `A` records point at GitHub Pages (185.199.108.153, 185.199.109.153,
185.199.110.153, 185.199.111.153) and `www` is a `CNAME` to `tarnsoftware.github.io`. The `MX` and other
email records belong to Microsoft 365 and must not be changed.
