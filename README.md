# Helix at ASHG 2026 landing page

A single-file, self-contained landing page for Helix's presence at the **ASHG 2026 Annual Meeting** (October 20-24, 2026, Palais des Congres de Montreal, Booth #1200).

The page previews the full Helix presence at the event: the featured plenary, platform talks, and posters; live Explorer platform demos (with a hub-and-spoke platform diagram); the Research Access Program; and the Sips and Genes networking reception. The primary call to action throughout is "Connect with our experts," which scrolls to an on-page interest form.

## Contents

- `index.html` - the complete landing page (HTML, CSS, and an inline SVG graphic in one file, no build step)
- `assets/` - reserved for images (for example, an official Helix logo PNG)
- `README.md` - this file

## Local preview

Open `index.html` directly in a browser, or serve it:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy with GitHub Pages

1. Go to **Settings > Pages**.
2. Under **Build and deployment**, set **Source** to *Deploy from a branch*, branch `main`, folder `/ (root)`.
3. Save. The page publishes at `https://jayshah-eng.github.io/helix-ashg-2026/`.

## Notes and customization

- **Interest form:** the connect section holds a styled interest form that is currently placeholder markup (it does not submit anywhere). Wire the `<form>` to your HubSpot form/portal, or set its `action` to the HubSpot endpoint, to capture submissions.
- **Calls to action:** every "Connect with our experts" button scrolls to the `#connect` form. Repoint them if you host the form elsewhere.
- **Reception details:** Sips and Genes reception is Wednesday, Oct 21, 2026, 5:30 to 7:30pm ET at Gazette Restaurant, Montreal.
- **Fonts:** the page loads Mulish from Google Fonts and falls back to system fonts offline.
- **Logo:** the header uses a text wordmark. Drop an official Helix logo PNG into `assets/` and wire it in if preferred (do not recreate the logo).
- **Content source of truth:** presentation titles, presenters, dates, times, and rooms come from the ASHG abstracts spreadsheet.

## Style

Colors, spacing, and typography mirror the live Helix events page (info.helix.com/ashg-2026) and the Helix brand system. The copy uses hyphens rather than em or en dashes throughout.

(c) 2026 Helix OpCo LLC. All rights reserved.
