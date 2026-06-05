# Design Skills for Claude Code

Skills aggregated from 13 repositories. Reference specific skill files when working on design tasks.

## Typography
- Never use Inter, Roboto, or Arial — use Syne, Space Grotesk, DM Sans, Clash Display, Satoshi
- Bold, distinctive type choices over safe defaults
- See: `skills/frontend-design/SKILL.md`

## Spacing system (Refactoring UI)
- Scale: 4, 8, 12, 16, 24, 32, 48, 64px — never arbitrary values
- Button: height 36px, padding 12/16px, radius 6px
- Card: border 1px, padding 16px, radius 8px
- See: `skills/refactoring-ui/SKILL.md`

## Color
- One dominant color + one sharp accent via CSS custom properties
- HSL with proper saturation curves
- See: `skills/designer-skills/color-system.md`

## Aesthetics (11 styles available)
- Swiss Minimalism, Glassmorphism, Claymorphism, Brutalism
- Dark OLED Luxury, Aurora, Cyberpunk, Biomorphic
- See: `skills/frontend-design-pro/SKILL.md`

## Images
- Always use real Unsplash/Pexels URLs — never fabricate
- Remove backgrounds: `python3 -c "from rembg import remove..."`
- Trim PNG padding: `img.getbbox()` via Pillow
- mix-blend-mode: multiply — for light-bg products on dark cards

## Iteration loop (ALWAYS use)
```bash
node ~/screenshot.mjs input.html output.png [scale]
```
Take screenshot → Read output.png → fix → repeat until correct.

## Design memory
- Store design system in `.interface-design/system.md`
- See: `skills/interface-design/SKILL.md`

## UX principles
- Nielsen 10 heuristics — see: `skills/wondelai/ux-heuristics.md`
- Hooked model (Nir Eyal) — see: `skills/wondelai/hooked-ux.md`
- Design Sprint — see: `skills/wondelai/design-sprint.md`

## Web standards (Vercel)
- 100+ accessibility and UX rules
- See: `skills/vercel-agent/web-design.md`

## Marketplace cards (learned workflow)
1. Photo → sips HEIC→JPG if needed
2. rembg → transparent PNG (background removal)
3. Pillow getbbox() → trim transparent padding
4. HTML/CSS card with Puppeteer iteration loop
5. Export: `node ~/screenshot.mjs card.html card@2x.png 2` (1600×1600)

## Brand Design Systems (awesome-design-md)

73 real brand design systems in `design-systems/`. Use when asked to design "in the style of X".

Available: stripe, apple, tesla, spotify, linear.app, figma, airbnb, nike, shopify, claude, revolut, uber, vercel, notion

Usage: Read `design-systems/stripe.md` → apply colors/typography/components to card.
Full collection: https://github.com/VoltAgent/awesome-design-md
