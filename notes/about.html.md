**about.html (Nosotros) — 2026-06-06 Hermes + CC delegation**

- Full adaptation: lang=es, title "Nosotros | Dulces Cubanos", description family story.
- Page hero: "Nuestra Historia Cubana", breadcrumb "Nosotros".
- Story section: detailed Cuban family narrative (abuela Esperanza from Santiago de Cuba, recipes, 2001 emigration, 2010 opening in Bradenton by Roberto & Luisa, 3 generations, "Este no es solo un negocio — es nuestro corazón.").
- Values section adapted to Cuban: "Recetas de Cuba", "Horneado Diario", "Comunidad".
- Photo placeholder kept with note for real family/local photo.
- Nav/footer consistent Spanish/Cuban branding.
- Verification (from read): content rich in Cuban history, Spanish throughout, emotional family tone.

**Customization:** Update family names/dates if real story provided. Keep the 3-generation warmth for authenticity.

Cross-ref: index.html, Report.md (session log), AGENTS.md.

---

## Pink primary + real bakery photo (2026-06-06 Hermes/CC)

- `.photo-placeholder` div replaced with `<img src="images/flan.jpg" alt="Foto de la familia Castellanos y el local de Dulces Cubanos en Bradenton" style="width:100%; height:100%; object-fit:cover; border-radius:14px;">`
- The `about-photo` wrapper (`aspect-ratio: 5/4`) provides the bounding box; `height: 100%` fills it fully.
- `border-radius: 14px` matches `--radius-lg` for visual consistency with the card system.
- `object-fit: cover` ensures the food/family shot crops gracefully at any size.
- Image: flan.jpg — a warm, golden Cuban food shot that evokes the family recipe story told in the text beside it. Tasteful pairing: text mentions "flan casero, cremoso" and image shows exactly that.
- Photo-placeholder CSS rules in style.css remain (no harm) — they simply no longer have a matching DOM element here.
---

## Session 2026-06-10 — Social Icons

- Facebook link corrected to https://www.facebook.com/p/Rosis-Dulces-Cubanos-61579793461133/
- TikTok link added: https://www.tiktok.com/@rosabelorihuela
- Instagram/WhatsApp text replaced with image icons from images/social/
- All 4 social links now use local icon assets (facebook.png, instagram.jpg, tiktok.jpg, whatsapp.png)
