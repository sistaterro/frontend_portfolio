# AGENTS.md - Frontend Portfolio

## Repository Purpose

This repository is a portable collection of frontend aesthetics and component sketches. It is not a production app, a shared design system package, or a single website. Each HTML file is a self-contained visual reference that can be opened directly in a browser, inspected, copied from, or moved into another project as inspiration or starting material.

The README acts as a storefront: it gives a quick visual catalog of the available aesthetics through PNG previews in `assets/`.

## Current Structure

- `README.md` - public catalog/storefront for humans browsing the collection.
- `AGENTS.md` - handoff guide for AI agents and maintainers.
- `assets/` - PNG preview images. Each preview should use the same base filename as its HTML page.
- `*.html` - self-contained aesthetic demos and component inventories.
- `debts.txt` - working backlog for design ideas, missing aesthetics, rough prompts, and future collection targets.

Current naming pattern:

```text
name.html
assets/name.png
```

Examples:

```text
hrcomponent.html
assets/hrcomponent.png

forum.html
assets/forum.png

ironworks.html
assets/ironworks.png

blackstone.html
assets/blackstone.png

atlas.html
assets/atlas.png

pulse.html
assets/pulse.png

newsroom.html
assets/newsroom.png

medcore.html
assets/medcore.png
```

## Maintenance Rules

- Keep each aesthetic self-contained unless the user explicitly asks for extraction into shared assets.
- Do not refactor multiple HTML files into a framework or shared build system without explicit direction.
- Preserve the visual identity of each page. These files are intentionally different from each other.
- When adding a new aesthetic, add both the HTML file and its matching PNG preview reference in `README.md`.
- If the PNG is not available yet, still add the expected `assets/name.png` reference if the user says they will provide it later.
- Keep README descriptions short and storefront-like: type, feel, best use cases, and visual signature.
- Treat `debts.txt` as a planning scratchpad. Update it only when the user asks to track, remove, or refine future aesthetic ideas.
- Prefer plain English documentation.
- Avoid changing filenames unless the user asks; filenames are part of the catalog contract.

## Handoff Notes For Other AI Agents

Before editing, inspect:

1. `git status --short`
2. `README.md`
3. The target HTML file
4. The matching image in `assets/`, if relevant
5. `debts.txt`, when the request involves future concepts, missing designs, or design planning

When a user asks to add a page to the catalog:

1. Confirm the HTML filename exists or infer the intended filename from the request.
2. Add `assets/<same-base-name>.png` to the image list in `README.md`.
3. Add a catalog card in `README.md` with concise aesthetic metadata.
4. Do not generate or modify the PNG unless explicitly asked.

When a user asks for a new aesthetic:

1. Create a standalone HTML file.
2. Give it a distinctive visual language.
3. Add a matching README card.
4. Reference the expected PNG in `assets/`.

## Current Aesthetics

- `hrcomponent.html` - SaaS / HR platform component system. Clean, professional, compact, dashboard-ready.
- `atlas.html` - Aerospace / robotics / defense mission-control design system. Deep navy, technical telemetry, precise and high-stakes.
- `blackstone.html` - Premium executive finance / investment design system. Charcoal, ivory, muted gold, formal and high-trust.
- `forum.html` - Forum / community media platform component system. Dark, loud, orange, condensed, social.
- `ironworks.html` - Manufacturing execution / industrial ERP design system. Dark steel, safety yellow, machine telemetry, plant-floor operations.
- `lumex.html` - Neon futurism / solar tech. Dark, glowing, particle-driven, premium tech.
- `medcore.html` - Healthcare / telemedicine / hospital operations design system. Clean medical blues, teal accents, accessible and calm.
- `newsroom.html` - Editorial / journalism / publishing design system. Warm paper, serif hierarchy, thin rules, credible and print-inspired.
- `nexusgrid.html` - Cyberpunk / high-tech infrastructure. Scanlines, glitch, telemetry, terminal visuals.
- `pulse.html` - AI startup / agent platform design system. Warm light SaaS surfaces, violet/mint accents, logs and workflow UI.
- `soltech_english.html` - Solar tech / clean industry. Warm, commercial, renewable-energy focused.
- `talkingdutch.html` - Institutional learning / Dutch language school. Sober, educational, local.
- `verdant.html` - Organic sustainability / solar product. Natural, soft, green, eco dashboard style.

## Commit Guidance

Keep commits small and descriptive. For catalog-only updates, a message like `Update aesthetic catalog docs` is enough. If adding a new HTML aesthetic and preview, mention the aesthetic name in the commit message.
