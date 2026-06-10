**services.html (Menú) — 2026-06-06 Hermes completion (CC partial + finish)**

- Full Spanish: "Menú | Dulces Cubanos", "Nuestro Menú Cubano", "Dulces Tradicionales".
- 6 service cards with authentic Cuban items + prices + descriptions:
  - Pastel de Guayaba $4.50
  - Flan Casero $5.75
  - Empanadas Cubanas $3.25 (3x$9)
  - Tres Leches $6.50 / $28 entero
  - Bizcochitos y Cafecito $2.75 + $2.50
  - Pedidos Especiales y Catering desde $45
- Descriptions emphasize "recetas de la abuela", "Santiago de Cuba", "La Habana", "quinceañeras", "calidez cubana".
- "Por qué elegirnos" section with Cuban values.
- Nav, hero, footer, CTA "Pedir ahora" / "Cotizar" in Spanish.
- Verification: complete menu in Spanish, realistic Cuban bakery offerings, prices, cultural notes.

**Customization:** Prices, exact menu items. Form action later to real endpoint.

Cross-ref: index.html, contact.html, style.css, Report.md.

**Note (2026-06-10):** Companion pricing note above is partially stale — "Pedidos Especiales y Catering desde $45" was updated by Hermes (2026-06-10 commit) to tiered pricing: Pequeño 10 porciones $57 / Mediano 20 porciones $78 / Grande custom consultar. The $45 figure no longer appears in the HTML.

---

## Pink primary + real bakery photos in service cards (2026-06-06 Hermes/CC)

Product images added to the top of 4 main service cards as bleed-edge banners:

| Card | Image |
|---|---|
| Pastel de Guayaba | images/guayaba-pastelito.jpg |
| Flan Casero | images/flan.jpg |
| Empanadas Cubanas | images/empanadas.jpg |
| Tres Leches | images/tres-leches.jpg |

**Implementation:** Each image wrapped in `<div style="margin: -2.25rem -2rem 1.5rem;">` — negative margins (-2.25rem top, -2rem left/right) bleed to the card's padding edges. `overflow:hidden` already set on `.service-card` clips cleanly with card's `border-radius: 14px`. Images at `height:160px; object-fit:cover; display:block; width:100%`.
Cards 5 (Bizcochitos) and 6 (Catering) retain Lucide icons — no matching prepared image.
Pink primary (#e75480) cascades via `--primary` to btn-outline borders, headings, card-link hover.
---

## Session 2026-06-10 — Social Icons

- Facebook link corrected to https://www.facebook.com/p/Rosis-Dulces-Cubanos-61579793461133/
- TikTok link added: https://www.tiktok.com/@rosabelorihuela
- Instagram/WhatsApp text replaced with image icons from images/social/
- All 4 social links now use local icon assets (facebook.png, instagram.jpg, tiktok.jpg, whatsapp.png)
