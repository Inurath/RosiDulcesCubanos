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