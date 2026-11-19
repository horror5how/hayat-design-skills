---
name: hayat-design-skills
description: Hayat's master design stack. Loads every design, motion, 3D, and anti-slop frontend skill he owns in the right order for any web design, redesign, landing page, animation, or brand visual task. Triggers - "design skills", "use my design skills", "Hayat's design skills", "make it look good", "redesign this", "build a landing page", "add animation", "make it beautiful", "non-AI look", "anti-slop".
---

# Hayat's Design Skills — master stack

One entry point for every design capability Hayat has installed. Do not pick one skill and stop.
Load the **core spine** every time, then add lanes by task type.

---

## 1. Core spine (ALWAYS load, in this order)

| Order | Skill | Why it goes here |
|---|---|---|
| 1 | `taste-skill:taste-skill` | v1.5 anti-slop frontend. Sets the design direction and the pre-flight check. This is the constitution — everything else obeys it. |
| 2 | `taste-skill:soft-skill` | Exact fonts, spacing, shadow, card, and motion values that read as expensive. Blocks cheap AI defaults. |
| 3 | `taste-skill:output-skill` | Kills truncation and `// rest of code here` placeholders. Without this the other skills get half-shipped. |
| 4 | `raylight` | Hayat's motion/design language, audited from raylight.app + jitter.video. Owns the cinematic feel. |
| 5 | `genjutsu:cast` | Interaction thesis + premium polish pass. Enforces "no code without a validated thesis". |

**Finance HQ rule still wins.** Any dashboard, metric surface, or data visual uses Finance HQ tokens
(see `feedback_visual_style_finance_hq` memory) regardless of what a style skill suggests.

---

## 2. Task lanes (add on top of the spine)

### Redesigning an existing site
- `taste-skill:redesign-skill` — audit-first, names the generic AI patterns before touching code
- `find-animation-opportunities` — read-only sweep for what should move and does not
- `improve-animations` / `review-animations` — fix motion that already exists
- **Never** rewrite generated output; edit the generator. See `be_redesign_revert_root_cause` memory.

### New landing page / marketing site
- `taste-skill:imagegen-frontend-web` — one horizontal reference image PER SECTION, never a combined board
- `taste-skill:image-to-code-skill` — generate the design image first, analyze deeply, then build to match
- `web-design-engineer`, `frontend-design`

### Motion + scroll
- `gsap-scrolltrigger` — pinning, stacking, scrub timelines
- `lottie-animations` — vector motion graphics, micro-icon animation
- `taste-skill:gpt-tasteskill` — strict GSAP ScrollTriggers, AIDA structure, gapless bento, wide editorial type
- `animation-designer`, `animation-vocabulary`

### 3D / WebGL
- `threejs-webgl` — immersive scenes, shader work, particle systems
- Budget rule: 3D is a hero-only device unless the product IS the 3D. Never 3D in three sections.

### Style direction (pick ONE, they conflict by design)
- `taste-skill:minimalist-skill` — warm monochrome, editorial, flat bento, no gradients
- `taste-skill:brutalist-skill` — Swiss print × military terminal, rigid grid, extreme type contrast
- `design-dna` — extract and recreate the DNA of a reference site Hayat points at

### Mobile / app screens
- `taste-skill:imagegen-frontend-mobile` — screens inside a subtle phone mockup
- `apple-design`, `ui-ux-pro-max`, `youtube-ux-specialist`

### Brand / identity
- `taste-skill:brandkit` — logo systems, brand-guideline boards, identity decks
- `taste-brandkit` (local install of the same)

### Design system handoff
- `taste-skill:stitch-skill` — generates an agent-readable DESIGN.md
- `theme-factory`, `design-html`

---

## 3. Non-negotiable rules for every design task

1. **Wireframe before pixels.** Show the structure — section order, hierarchy, what the eye hits first — before writing a line of CSS. Hayat asks for this explicitly and it is the fastest way to catch a wrong direction.
2. **Anti-AI-look pre-flight.** Before shipping, confirm none of these are present:
   - purple→blue gradient hero
   - three identical feature cards in a row with a lucide icon on each
   - `Inter` + generic 8px-radius card + `shadow-lg` everywhere
   - centered-everything with no asymmetry
   - stock "abstract tech" imagery
   - em-dash-heavy body copy and "Unlock the power of…" headlines
3. **No new dependency without asking.** Native platform APIs and already-installed libs first.
4. **60fps or cut it.** Animate transform and opacity only. Never width, height, top, left.
5. **Reduced motion respected** on every animation, always.
6. **Verify with Playwright before saying done.** Screenshot proof, per `feedback_playwright_qa`.
7. **Real photos of Hayat, never AI-generated portraits.** See `feedback_no_ai_photos`.

---

## 4. Where these live

- Taste suite repo: `~/.claude/skills/taste-skill` (registry, `git pull` to update). Also installed standalone as `~/.claude/skills/taste-*`. See `taste_skill_suite` memory.
- Genjutsu, gsap-scrolltrigger, lottie-animations, threejs-webgl: Claude Code plugins.
- Raylight, design-dna, web-design-engineer: `~/.claude/skills/`.

Source of the 5 motion/3D skills: IG post by @olaconleyy (2026-07-21). Taste suite: @chase.h.ai reel (2026-06-28).
Related: [[taste_skill_suite]] · [[raylight skill motion design]] · [[feedback_visual_style_finance_hq]] · [[feedback_playwright_qa]]
