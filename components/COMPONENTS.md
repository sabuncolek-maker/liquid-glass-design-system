# Components — Liquid Glass Design System

Every component shares: angular cut-corner geometry (one consistent cut size), glass material per the level noted, thin luminous border, consistent spacing (8 px base), and the states Default / Active / Transition. Hover applies only where the medium supports it.

## Glass Material Recipe (all glass components)

- Semi-transparent surface over a blurred copy of the background (frosted).
- Subtle metallic reflection: a soft diagonal light gradient, plus an optional slow reflection sweep in motion.
- Thin luminous border: silver at rest, electric blue edge glow for focus/active.
- Layered transparency: never fully opaque, never so transparent that text loses readability.

## 1. Glass Panel
Main content container. Glass Dark or Glass Light. Diagonal cuts on all four corners. Holds headings (Space Grotesk) and body (Inter).

## 2. Angular Card
Smaller information unit. Same cut-corner system as the panel, Glass Light by default, blue edge glow when it carries the scene's key number or fact.

## 3. Primary Button
Glass Accent (blue translucent) with solid blue focus state. Inter SemiBold label. Angular shape, small cut.

## 4. Secondary Button
Glass Light, silver border, white label. Blue glow only in active state.

## 5. Navigation Bar
Horizontal Glass Dark bar, angular ends. Icons are geometric outlines; the active item sits in a blue glass pill.

## 6. Glass Icon Button
Square angular glass tile, geometric outline icon in silver/white; blue tile when active.

## 7. Toggle Switch
Angular track (Glass Dark), silver knob; on-state fills the track with Electric Blue and adds a soft cyan highlight.

## 8. Progress Indicator
Thin angular track (Glass Dark) with a liquid fill: gradient Electric Blue → Cyan Glow → Light Silver, glowing leading edge.

## 9. Glass Modal
Centered Glass Light panel over a dimmed, blurred scene. Blue edge glow. Enters with Panel Reveal motion (500–800 ms).

## 10. Information Panel
Glass Dark side panel for supporting data: small Inter labels, Space Grotesk values, blue highlight for the key figure.
