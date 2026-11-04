---
name: liquid-glass-design-system
description: Apply the Liquid Glass Futuristic design system (Silver × Black × Electric Blue, angular glass) when designing or animating motion graphics and UI. Use whenever producing visuals in this style.
---

# Liquid Glass Design System — Agent Instructions

You are producing motion graphics / UI visuals in the Liquid Glass Futuristic style owned by Erlangga. The full specification lives in `DESIGN-SYSTEM.md` in this repository — read it before producing anything. Machine-readable values live in `tokens/design-tokens.json` and `tokens/tokens.css`. Component specifications live in `components/COMPONENTS.md`.

## Hard rules

- Palette is frozen: Electric Blue `#0D6EFD`, Silver `#C0C4CC`, Deep Black `#0B0B0D`, plus the supporting tokens in the design system. Distribution 50% black/navy, 25% silver, 15% blue, 10% white/cyan. Never introduce new main colors or random gradients.
- Geometry is angular: diagonal cut corners, one consistent cut size. Oversized rounded corners are forbidden.
- Fonts: Space Grotesk for headings, Inter for body. Nothing else.
- Glass material on every panel/card: frosted transparency, metallic reflection, thin luminous border, layered depth (Glass Light / Glass Dark / Glass Accent).
- Motion is smooth and controlled, using the duration table in the design system. No fast, broken, or excessive movement; no excessive glow.
- Visual consistency beats decorative effects. Never sacrifice readability for an effect.
- No cartoon elements mixed into the futuristic style. No decorative element without a function. Every scene keeps the same design identity.

## Workflow

1. Read `DESIGN-SYSTEM.md` and the tokens.
2. Build or reuse the components — never redesign a component per scene.
3. Storyboard the scenes (opening → main content → transitions → closing) per section 9 of the design system.
4. Build an animatic / preview first and get it approved before the final render.
5. Produce the final animation.
6. Consistency check before delivery: colors, fonts, corner system, lighting, motion timing — all against the tokens.

## Scene composition

- Opening: dark navy background, blue light streak, glass elements appear gradually (layer reveal + parallax).
- Main content: Space Grotesk headings, Inter information, liquid glass panels, Electric Blue highlights.
- Transitions: angular masks, glass reflection sweeps, parallax. Keep visual continuity.
- Closing: restate the key information, blue glow accent, clean exit transition.
