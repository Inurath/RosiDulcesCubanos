# Dulces Cubanos Website — Project AGENTS (CC / Hermes / Future Agents)

**Project root:** `/home/randy/Documents/Web Agency/Dulces Cubanos Website/`  
**Live goal:** Static multi-page website for Dulces Cubanos, authentic local Cuban bakery. Fully in Spanish, vibrant Cuban culture and flavors. Adapted from professional template for quick client delivery.  
**Main objective:** Deliver professional, ready-to-deploy static HTML/CSS/JS sites matching the agency's Professional tier. Part of Web Agency multi-project system.

---

## Mandatory Startup (Every Session)
1. Read this `AGENTS.md`.
2. Read `Report.md` (current state, decisions, logs, handoff notes).
3. `ls -la` the folder + check git status.
4. Check `/home/randy/Documents/Personal/CLI Core/CLI Tasks.md` and `/home/randy/Documents/Web Agency/Web Tasks.md` for related tasks.
5. Check parent `/home/randy/Documents/Web Agency/AGENTS.md` for global rules.

---

## Core Rules
- **Document everything:** For every file created/edited, immediately create/update companion note in `notes/<filename>.md` (purpose, key changes, customization guide, Cuban-specific decisions).
- **Report.md is the single source of truth.** Append structured session log on every turn (trigger, actions with tool outputs, verification, handoff).
- **No user exec:** Do all work yourself (edits, git, verification). Preview by opening HTML in browser.
- **End of every session:** Update Web Tasks.md + Log Web Tasks.md if applicable. Run `dotfiles-sync save`. Commit/push the project repo. Update main CLI Reports if this was from CLI Tasks pending.
- **Verification always:** After changes: manually inspect key sections (hero, menu, about, contact), test theme toggle, responsive, Spanish completeness. Note browser preview results.
- **Tech Stack:** Pure static HTML5 + CSS + JS (no build step, open index.html directly). Matches Professional template: 5 pages, schema, dark/light theme, Lucide icons, responsive nav, forms with mailto fallback.
- **Customization for clients:** All variables in style.css :root for easy retheme. Copy-paste pattern from professional template. Future clones: replace business details, menu, photos (placeholders), socials.
- **Cuban Bakery specifics (this project):** All copy in Spanish. Content celebrates Cuban heritage: family recipes from Cuba, traditional dulces (pasteles, flan, empanadas, tres leches, etc.), warm community vibe, "Hablamos Español", Florida local (Bradenton/Sarasota/Miami area). Colors: vibrant yet professional (Cuban flag reds/golds/blues with warm accents).
- **Git + GitHub:** Sensible commits. Repo: Inurath/dulces-cubanos-website (or similar). Good README. Link in main vault.
- **Second brain:** This folder + Report + notes/ live in Web Agency vault. Link from Personal/Home.md, Dashboard, CLI Tasks when active.

---

## Recommended Workflow
1. Update todo (internal or in Report).
2. Read target files + companions + Report.
3. Make edits (read first, then precise changes for Spanish/Cuban theme).
4. Immediately: companion note + append to Report.md.
5. Verify: open index.html in browser (or python -m http.server), check all pages, theme, mobile.
6. Commit (small, descriptive, in Spanish/English mix as needed).
7. At milestones: update Web Tasks if tracked, push repo, dotfiles-sync, main logs.
8. Handoff: clear sections in Report for next agent (CC/Hermes).

---

## Quick References
- Folder: `/home/randy/Documents/Web Agency/Dulces Cubanos Website/`
- Preview: open `index.html` in any browser (no server needed for static).
- Git remote target: https://github.com/Inurath/dulces-cubanos-website
- Accent inspiration: Cuban flag (#c8102e red, white, #002a8f blue) + warm golds.
- Parent rules: `/home/randy/Documents/Web Agency/AGENTS.md`
- Eternal reference: `/home/randy/Documents/Web Agency/eternalwebsite.com/AGENTS.md` (for log structure).

**This file + Report.md + notes/ are the contract.** Follow for seamless handoff.

*Created 2026-06-06 by Hermes + CC delegation during "read your notes and do your tasks" per CLI Tasks pending.*