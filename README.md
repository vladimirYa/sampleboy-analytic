# Sampleboy Analytics

Static, private usage dashboard for Sampleboy. The dashboard is published at:

https://vladimirya.github.io/sampleboy-analytic/

It contains no stored event data. To load statistics, enter the HTTPS Worker API
origin and the dashboard token configured as `ANALYTICS_ADMIN_TOKEN` in Cloudflare.
The token is used in memory for the request and is not saved in browser storage.

## GitHub Pages

In this repository's **Settings → Pages**, publish the `main` branch from the
root directory. GitHub Pages then serves `index.html` at the URL above.

## Analytics API

The event API and database are deployed separately as a Cloudflare Worker with a
D1 binding. Deployment steps and the event schema are maintained in the Sampleboy
extension repository under `analytics-api/README.md`.

The dashboard shows only opt-in aggregate events. The privacy policy is at
https://vladimirya.github.io/audio-recorder-sample-slicer-pp/.
