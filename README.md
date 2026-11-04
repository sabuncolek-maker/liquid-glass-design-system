# Liquid Glass Design System

Futuristic design system for motion graphics and UI animation.
**Liquid Glass + Angular Geometry** — Silver × Black × Electric Blue.

Author: Erlangga · Version 1.0 · License: MIT

## Identity

- Visual style: Liquid Glass (frosted transparency, metallic reflection, luminous edges)
- Geometry: Angular — sharp, chamfered, cut-corner shapes. No oversized rounded corners.
- Mood: Modern, professional, futuristic, premium.
- Priority: Visual consistency > decorative effects. Never sacrifice readability for effects.

## Palette

| Token | Color | Hex | Role |
|---|---|---|---|
| Primary Blue | Electric Blue | `#0D6EFD` | Highlight, CTA, visual focus |
| Secondary Silver | Silver | `#C0C4CC` | Panels, borders, secondary elements |
| Base Black | Deep Black | `#0B0B0D` | Main background |
| Dark Navy | Navy | `#080E1B` | Background support |
| Light Silver | Light Silver | `#E2E7F0` | Light surfaces, text support |
| White | Pure White | `#FFFFFF` | Primary text |
| Cyan Glow | Electric Cyan | `#00CFFF` | Lighting accent only |
| Dark Surface | Glass Dark | `#18243A` | Dark glass material |

Distribution: 50% Black / Dark Navy · 25% Silver · 15% Electric Blue · 10% White / Cyan Glow.
Never use all colors at the same intensity.

## Typography

- Headings: **Space Grotesk** (700 / 600 / 500)
- Body: **Inter** (400 / 500 / 600)
- Never more than two font families. No decorative fonts.

## Geometry

- Panels use diagonal cut corners, applied consistently across all components.
- Buttons and cards use firm geometric shapes and angular outlines.
- One corner system for the whole system.

## Glass Material

Three levels: **Glass Light** (silver translucent), **Glass Dark** (dark transparent), **Glass Accent** (blue translucent).
Every glass element: semi-transparent surface, background blur, subtle metallic reflection, thin luminous border (electric blue edge glow), layered transparency.

## Motion

Smooth, precise, controlled. Fade In · Slide In · Scale Transition · Glass Reflection sweep · Blue Glow Pulse · Layer Reveal · Parallax.

| Type | Duration |
|---|---|
| Micro interaction | 150–250 ms |
| UI transition | 300–500 ms |
| Panel reveal | 500–800 ms |
| Scene transition | 600–1000 ms |

## Repository Structure

- `DESIGN-SYSTEM.md` — the complete master document (philosophy, color, typography, geometry, glass, components, spacing, motion, composition, consistency rules).
- `tokens/` — machine-readable design tokens (`design-tokens.json`, `tokens.css`).
- `components/` — reusable component specifications.
- `SKILL.md` — instructions for AI agents: how to apply this system when producing animations.
- `examples/` — visual references and style tests.

## For AI Agents

Read `SKILL.md` first, then `DESIGN-SYSTEM.md`. Build tokens, build reusable components, storyboard, animatic, final render, consistency check — in that order.

## License

MIT — see `LICENSE`.
