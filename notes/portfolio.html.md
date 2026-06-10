**portfolio.html (Galería) — 2026-06-06 Hermes completion**

- "Galería | Dulces Cubanos", "Nuestra Galería de Dulces", "Especiales de la Casa".
- 4 portfolio cards with emoji placeholders + descriptions:
  - Pastel de Guayaba (Clásico, Más vendido)
  - Flan de la Abuela (Favorito familiar)
  - Empanadas (Salado o dulce, Para llevar)
  - Tres Leches Especial (Celebraciones, Personalizable)
- Tags in Spanish, meta like "Desde 2010", "Receta de la abuela".
- Call to action to contact or visit for more/real photos.
- Fully Spanish, Cuban pride in copy ("el sabor de Cuba", "quinceañeras y cumpleaños cubanos").
- Verification: structure matches professional, content 100% Spanish + cultural.

**Customization:** Add more cards or customer testimonials as real photos become available.

Cross-ref: services.html, contact.html, AGENTS.md.

---

## Pink primary + real bakery photos (2026-06-06 Hermes/CC)

All 4 `.portfolio-image` divs updated — gradient backgrounds and emoji placeholders replaced with real food images:

| Card | Image | Alt text |
|---|---|---|
| Pastel de Guayaba | images/guayaba-pastelito.jpg | Pastel de Guayaba |
| Flan de la Abuela | images/flan.jpg | Flan de la Abuela |
| Empanadas | images/empanadas.jpg | Empanadas |
| Tres Leches Especial | images/tres-leches.jpg | Tres Leches Especial |

**Implementation:** Each `.portfolio-image` gets `style="position:relative; background:none;"` with the inner `<img>` at `width:100%; height:210px; object-fit:cover; display:block;` — matches original div height, scales responsively, clips cleanly.
Old inline gradient styles (`#c8102e`, `#d4a017`, `#002a8f`) removed.
Pink primary (#e75480) via `--primary` cascades to filter buttons (active state), portfolio-price text, `::before` hover gradient bar.
Note: this portfolio.html uses a simplified footer (`.footer-grid` not `.footer-inner`) — kept as-is, consistent with services.html pattern.
---

## Session 2026-06-10 — Social Icons

- Facebook link corrected to https://www.facebook.com/p/Rosis-Dulces-Cubanos-61579793461133/
- TikTok link added: https://www.tiktok.com/@rosabelorihuela
- Instagram/WhatsApp text replaced with image icons from images/social/
- All 4 social links now use local icon assets (facebook.png, instagram.jpg, tiktok.jpg, whatsapp.png)
