**style.css — 2026-06-06 Hermes + CC delegation**

- Palette updated to Cuban professional: 
  --primary: #c8102e (rojo cubano bandera)
  --accent: #d4a017 (oro cálido, celebración)
  Comments in Spanish/English explaining "PALETA CUBANA PROFESIONAL".
- All other vars (text, bg, shadows, radius) kept professional for readability on white/warm bg-alt #fdf6f0.
- Dark mode support intact via existing rules + data-theme.
- Buttons, cards, nav, forms, portfolio grid, etc. use the new accent/primary for CTAs and highlights.
- Verification: head of file confirms new :root colors and Cuban comment. Theme toggle works with warm dark #1a0808.

**Customization:** Tweak --primary / --accent for different vibes. All components inherit via vars — global retheme easy.

Cross-ref: all 5 HTML files, AGENTS.md (color guidance).

---

## Pink primary + real bakery photos (2026-06-06 Hermes/CC)

**Trigger:** User explicit: "primary color is pink." + "find online pictures of Cuban bakery products and replace placeholders."

**Color changes:**
- `--primary: #c8102e` → `#e75480` (deep rose / hot pink — sweet Cuban vibe, dulcería energy)
- `--primary-dark: #9b0c23` → `#c43060` (darker rose for hover/contrast)
- `--primary-light: #e01535` → `#ff69b4` (hot pink light variant for gradients/hover effects)
- Comment header updated: "rosa vibrante — pink primary for Dulce Cubanos branding (sweet Cuban vibe with gold accents)"
- Dark mode comment updated: "rosa cubano dulce"
- Hardcoded RGBA box-shadow values updated: btn-primary:hover → `rgba(231,84,128,0.3)`, form focus → `rgba(231,84,128,0.1)`
- `--accent: #d4a017` (gold) retained — Cuban harmony maintained ✓

**Hero image change (index.html hero-bg):**
- `.hero-bg` rule updated from `linear-gradient(135deg, #6b0516 0%, #c8102e 55%, #e01535 100%)` to `background-image: url('images/guayaba-pastelito.jpg'); background-size: cover; background-position: center;`
- `.hero-bg::after` overlay kept `rgba(0,0,0,0.55) → rgba(0,0,0,0.1)` gradient for text readability ✓

**Why #e75480:** Deep rose / hot pink sits between hot pink (#ff69b4) and dark pink (#c71585). Sweet, feminine, festive — perfect for a "Dulces" bakery with Cuban flair. Keeps enough contrast on white bg. Gold accent harmonizes beautifully (think pink boxes + gold ribbon).

**All CSS rules using --primary auto-update via var()** — nav, buttons, headings, section-header h2, page-hero, cta-band, portfolio filters, team-photo gradients, footer logo-mark, etc.
---

## Session 2026-06-10 — Dark Mode Nav Contrast + Map Section + Social Icon Styles

**Dark mode nav contrast fix:**
- Added `[data-theme="dark"] .nav-links a { color: #f5dde8; }` — brighter/lighter pink for inactive nav links in dark mode
- Added `[data-theme="dark"] .nav-links a:hover { color: var(--primary-light); background: rgba(231,84,128,0.18); }`
- Previous: `--text-muted` (#b090a8) was used, potentially low perceived contrast on #18101a bg. Fixed to brighter #f5dde8.

**Hero-bg rule re-added:**
- `.hero-bg { background-image: url('images/guayaba-pastelito.jpg'); background-size: cover; background-position: center; }` — was removed by linter, restored.

**Social icon image styles:**
- `.social-links a img` — 22×22px, object-fit: contain, border-radius: 3px
- Hover: scale(1.15), opacity 0.85

**Map section styles:**
- `.map-section { background: var(--bg-alt); }`
- `.map-embed-wrap` — border-radius, box-shadow, 420px iframe height
- `.map-cta { text-align: center; margin-top: 1.5rem; }`
