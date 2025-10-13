# GOES-19 SMV GeoColor – Live Satellite Add-in Bundle

**What this is:** A minimal PowerPoint **Content add-in** that embeds a web page you host on GitHub Pages. That page shows the NOAA STAR GOES-19 Southern Mississippi Valley GeoColor image and auto-refreshes.

## Files
- `live-sat/index.html` – renders the image and auto-refreshes (default every 5 minutes).
- `live-sat/icon-32.png`, `live-sat/icon-64.png` – placeholder icons.
- `manifest.xml` – the add-in manifest that PowerPoint uses.

## How to publish
1. In your GitHub repo `MattTheMet`, create a folder `live-sat/` and upload the three files from this folder into it.
   - Your page will be at: `https://mattisback04.github.io/MattTheMet/live-sat/`
2. In **PowerPoint on the web** open your deck → **Insert → Add-ins → My Add-ins → Upload My Add-in** → select `manifest.xml`.
3. Insert the add-in onto a slide and resize as needed.

## Change refresh cadence
Open `index.html` and adjust the input default value (seconds) or the timer interval in JS.

## Image source
`https://cdn.star.nesdis.noaa.gov/GOES19/ABI/SECTOR/smv/GEOCOLOR/latest.jpg` – this `latest.jpg` is updated by NOAA STAR every 5–10 minutes for the SMV sector.
