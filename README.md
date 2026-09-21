# Recco

Source for the Recco marketing site — homepage (`index.html`) and `what-we-do.html`, plus the favicon set and the social share image.

## Before this is really live

Open `index.html` and `what-we-do.html` and edit the five lines at the top of each `<script>window.RECCO = {...}</script>` block:

```js
window.RECCO = {
  WEBHOOK_URL: "",              // paste an n8n / Make / Zapier catch-hook URL here
  EMAIL:       "hello@recco.co",// your real, monitored inbox
  PHONE:       "",              // optional -- leave "" to hide
  CITY:        "Rexburg, Idaho",
  DOMAIN:      "recco.co",
  TURNAROUND:  "one business day"
};
```

Until `WEBHOOK_URL` is filled in, the form falls back to opening the visitor's own email app addressed to `EMAIL` — it works, but it's the fallback, not the real thing.

## Publishing with GitHub Pages

Settings → Pages → Deploy from a branch → `main` / `/ (root)` → Save. GitHub gives you a `https://<username>.github.io/<repo>/` URL a minute or two later. A custom domain can be added later from that same Pages settings screen — no changes to these files needed until then.
