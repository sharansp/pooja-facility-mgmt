# Design Guidelines

## Colour palette (current — keep as-is)
| Token | Value | Usage |
|---|---|---|
| `--navy` | `#0d2647` | Primary dark, headings, nav background |
| `--navy-2` | `#123763` | Hover states, gradients |
| `--navy-3` | `#0a1d38` | Dark sections, footer, contact card |
| `--green` | `#5a9e2f` | Primary CTA, accents, checkmarks |
| `--green-2` | `#75b647` | Hover on green buttons |
| `--teal` | `#2f8fb0` | Secondary accent, tags |
| `--bg` | `#f6f8fa` | Page background, alternating sections |
| `--card` | `#ffffff` | Card backgrounds |
| `--text` | `#1c2530` | Body text |
| `--muted` | `#5b6472` | Secondary text, descriptions |
| `--line` | `#e6eaef` | Borders, dividers |

## Typography
- Headings: `Poppins` 700/800
- Body: `Inter` 400/500/600
- Base size: 16px, line-height 1.65
- Heading scale: `clamp()` for fluid sizing

## Spacing
- Section padding: `96px 0` (desktop), `64px 0` (≤640px)
- Container max-width: `1180px`, horizontal padding `24px`
- Card padding: `30px 24px`
- Border radius: `--radius: 14px` for cards, `10px` for buttons, `999px` for pills/chips

## Shadows
- Default: `0 10px 30px rgba(13,38,71,0.08)`
- Large: `0 20px 50px rgba(13,38,71,0.16)`

## Buttons
- `.btn-primary` — green background, white text
- `.btn-outline` — transparent, white border (on dark backgrounds)
- `.btn-navy` — navy background, white text
- All buttons: `padding 15px 30px`, `border-radius 10px`, `font-weight 600`

## Responsive breakpoints
- `≤980px` — tablet: single-column grids, hide desktop nav, show burger
- `≤640px` — mobile: reduced section padding, 2-col or 1-col grids

## Animations
- Scroll reveal: `.reveal` → `.reveal.in` via IntersectionObserver (opacity + translateY)
- Hover on cards: `translateY(-6px)` + larger shadow
- Header: transparent → navy on scroll
- Keep animations subtle — no excessive motion
