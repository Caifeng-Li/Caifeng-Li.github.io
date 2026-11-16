# Activate the visitors map

The website is ready for a real visitor map. **No fake visitor totals are displayed.** Since GitHub Pages is static hosting, a third-party map service must track and aggregate visits.

1. Visit https://statflag.com/ and create a free map for `https://caifeng-li.github.io/`.
2. After creating the map, copy the iframe embed code the service gives you.
3. Find the `src="https://..."` URL inside that iframe code. Copy the **URL only**, not the entire HTML tag.
4. Open `visitor-map-config.js`, replace the empty string on `window.CAIFENG_VISITOR_MAP_URL = "";` with that URL.
5. Upload `visitor-map-config.js` (and this website version if you haven't already uploaded it) to your GitHub Pages repository, `Caifeng-Li/Caifeng-Li.github.io`, and commit.
6. Open https://caifeng-li.github.io/ and refresh. Your map will appear in the Visitors section. Counts normally begin from when the widget starts tracking, not when the site was originally created.

The provider is external and may use IP geolocation or other means to estimate visitors' countries. Avoid making privacy claims not confirmed in the provider's privacy policy. An iframe may be blocked by restrictive browser settings. The original design in the screenshot is not necessarily a StatFlag widget, so this is a comparable embedded solution rather than an exact copy.

**Tip:** Keep the iframe URL in this config file; do not paste script tags or API secrets.
