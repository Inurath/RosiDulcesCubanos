**index.html (Home) — 2026-06-06 Hermes + CC delegation**

- Adapted from professional template base (copied by Hermes).
- Full Spanish + Cuban theme: title "Dulces Cubanos | Panadería y Dulcería Cubana Auténtica — Bradenton, FL", hero badge Bradenton, hero text about authentic Cuban sweets, quick services strip with pastries teaser, stats in Spanish ("+10 años", "Recetas de la abuela", etc.).
- Schema updated to Bakery with Cuban details, address Bradenton, servesCuisine "Cuban".
- Nav, buttons, footer all Spanish ("Inicio", "Menú", "Contáctanos", "Hablamos Español").
- Theme toggle label "Cambiar modo oscuro".
- Colors reference Cuban palette (red/gold from style.css).
- Cuban elements: guayaba, flan, empanadas, cafecito mentions in hero/services teaser; family warmth copy.
- Verification: head read confirmed lang=es, Spanish content, Cuban specifics. Open in browser to preview hero + nav + quick menu.

**Customization notes:** Change address/phone in schema + footer. Update hero stats or menu teasers in the HTML. Colors via style.css :root. Photos: replace placeholders.

Cross-ref: AGENTS.md, Report.md, services.html, about.html.

---

## Pink primary + real bakery photos (2026-06-06 Hermes/CC)

- Hero `.hero-bg` now shows `images/guayaba-pastelito.jpg` (a real food photo) via style.css update — no inline style change needed in this HTML file.
- Dark overlay (`::after`) retained for text legibility: left-side dark gradient fades out right.
- Pink primary (#e75480) cascades to all nav elements, CTA band, stat numbers via --primary var.
- index.html itself unchanged — all color/image updates in style.css only.

---

## Session 2026-06-10 — CC Verification Pass: Copyright + Footer Consistency

**Copyright year:** Fixed `&copy; 2025` → `&copy; 2026` in footer-bottom.
**Footer Visítanos:** Added `<p class="contact-line">Mié–Vie 4PM–9PM<br>Sáb–Dom 1PM–9PM</p>` after email — all 5 pages now consistently show address, phone, email, and hours in footer.

---

## Session 2026-06-10 — Map Section + Social Icons

**Map section added (before </main>):**
- New `<section class="map-section section">` with Google Maps iframe embed
- Source: `https://maps.google.com/maps?q=5507+14th+St+W+Bradenton+FL+34207&output=embed&z=15`
- Section header: "Dónde Estamos / Encuéntranos en Bradenton"
- "Abrir en Google Maps" btn-outline button linking to place query
- Responsive via `.map-embed-wrap` + `iframe { width:100%; height:420px }`

**Social links footer:**
- Facebook updated to `https://www.facebook.com/p/Rosis-Dulces-Cubanos-61579793461133/`
- Added TikTok: `https://www.tiktok.com/@rosabelorihuela`
- All 4 icons now display image assets from `images/social/`

---

## Session 2026-06-10 — Owner Portrait as Logo + Hero Background

**Request:** Use `images/rosi.jpg` as the site logo and main homepage hero background.

**Logo change (all 5 pages):**
- Replaced the old `.logo-mark` monogram with `<img src="images/rosi.jpg" alt="Dulces Cubanos" class="logo-img">` in nav + footer brand blocks
- Sizing: 48×48px, `object-fit: cover`, rounded corners for a clean brand mark

**Hero background change (index.html + internal pages):**
- `style.css` now sets the main `.hero` background to `images/rosi.jpg`
- Added `.hero::after` gradient overlay so text stays readable over the portrait
- Disabled the old `.hero-bg` rule/photo to avoid double backgrounds
- Internal page `.page-hero` also uses the same portrait with a darker overlay and lifted text via `z-index`
