# CDI Solutions — Style Guide

## Colours

| Token | Value | Usage |
|---|---|---|
| Background | `#000000` / `#0d0d0d` | Page background, nav, dark sections |
| Surface dark | `rgba(255,255,255,0.03)` | Subtle card fills |
| Text primary | `#ffffff` | Headings, body on dark |
| Text faded | `rgba(255,255,255,0.55–0.65)` | Body copy, subtext |
| Text muted | `rgba(255,255,255,0.3–0.4)` | Footer copy, placeholders |
| Accent / Brand | `#f97316` | Buttons, highlights, chips, eyebrows |
| Accent hover | `#ea6a0a` | Button hover state |
| Light bg | `#f7f9fc` | Projects section (white background) |
| Text on light | `#0a1628` | Headings on white bg |
| Border subtle | `rgba(255,255,255,0.08–0.1)` | Dividers, card borders |
| Border medium | `rgba(255,255,255,0.3)` | Button outlines |

---

## Headings

**No eyebrow text above section headings.** Section titles stand alone — do not add uppercase label/chip text (e.g. "Our Services", "What We Do") above `h2` or `h3` headings on the main page. Eyebrow chips are only used inside the Our Approach section as a deliberate design accent.

---

## Typography

**Font family:** `"PP Mori", Arial, sans-serif`

### Scale

| Level | Size | Weight | Line height | Letter spacing | Usage |
|---|---|---|---|---|---|
| Display | `clamp(3rem → 4.5rem)` | 800 | 1 | 0 | Hero headline |
| H1 | `5rem` | 800 | 1.2 | 0 | — |
| H2 | `3.75rem` | 800 | 1.2 | −0.02em | — |
| H3 | `3rem` | 800 | 1.1 | −0.02em | Section headings (Sectors, Projects, Who We Are, Our Approach) |
| H4 | `2.375rem` | — | 1.2 | — | — |
| H5 | `2rem` | — | — | — | — |
| H6 | `1.5rem` | — | — | — | — |
| Body main | `1rem` | 400 | 1.5 | 0 | Paragraphs |
| Body large | `1.125rem` | 400 | 1.75 | 0 | Lead copy |
| Body small | `clamp(0.65rem → 0.85rem)` | 400 | — | — | Captions, labels |
| Eyebrow | `0.68–0.75rem` | 700 | — | 0.12–0.14em | Uppercase chip labels |
| Card title | `1.75rem` | 700 | 1.2 | −0.02em | Project card title, sector card title |
| Card meta | `1rem` | 400 | — | 0 | Sector · location line |

### Font weights in use
- `400` — regular body
- `500` — medium (nav links, button secondary)
- `600` — semibold (buttons primary, eyebrows)
- `700` — bold (card titles, button text)
- `800` — extrabold (section headings)
- `900` — black (approach pillar numbers)

---

## Spacing

### Gap scale

| Token | Value |
|---|---|
| gap-1 | `0.25rem` |
| gap-2 | `0.5rem` |
| gap-3 | `0.75rem` |
| gap-4 | `1rem` |
| gap-5 | `1.5rem` |
| gap-6 | `2rem` |
| gap-7 | `3rem` |
| gap-8 | `4rem` |
| gap-9 | `5rem` |
| gap-10 | `6rem` |
| gap-12 | `8.5rem` |

### Section padding
- Default (main): `7rem` top + bottom
- Compact: `5rem` top + bottom (approach inner)
- Light: `3.5rem` (who we are)
- Horizontal page padding: `1.5rem` (mobile) → `2.5rem` (desktop) → constrained to `1200px` max-width

### Container
- Max content width: `1200px`, centred with `margin: 0 auto`

---

## Border Radius

| Token | Value | Usage |
|---|---|---|
| Small | `0.75rem` | Buttons, chips |
| Main | `1.25rem` | Cards, images, image blocks |
| Round | `100vw` | Pill badges |

---

## Borders

- Default border width: `~0.094rem` (≈1.5px)
- Card border: `1px solid rgba(255,255,255,0.1)`
- Divider: `1px solid rgba(255,255,255,0.08)`
- Button border (outline): `2px solid rgba(255,255,255,0.75)`
- Accent border (chip): `1px solid rgba(249,115,22,0.3)`

---

## Components

### Navigation
- Position: `sticky`, `top: 0`, `z-index: 100`
- Height: `72–80px`
- Background: `#000000`
- Border bottom: `1px solid rgba(255,255,255,0.08)`
- Logo height: `44px`
- Padding: `0 2.5rem` (mobile: `0 1.25rem`)

### Buttons — Primary
```
background: #f97316
color: #fff
padding: 1rem 1.5rem 0.9rem
border-radius: 0.75rem
font-weight: 600
font-family: "PP Mori", Arial, sans-serif
transition: background 0.2s
hover background: #ea6a0a
```

### Buttons — Outline (on dark)
```
background: transparent
border: 2px solid rgba(255,255,255,0.75)
color: #fff
padding: 1rem 1.5rem 0.9rem
border-radius: 0.6rem
font-weight: 700
letter-spacing: -0.02em
```

### Sector Cards
- Size: `270px × 370px`
- Border radius: `1.25rem`
- Border: `1px solid rgba(255,255,255,0.1)` → hover `rgba(249,115,22,0.4)`
- Image: full-bleed `position: absolute; inset: 0; object-fit: cover`
- Overlay: `linear-gradient(to top, rgba(8,8,8,0.85) 0%, rgba(8,8,8,0.3) 50%, transparent 100%)`
- Content area: `padding: 1.25rem 1.5rem 1.5rem`, `background: rgba(8,8,8,0.75)`, `border-top: 1px solid rgba(255,255,255,0.1)`
- Title: `1.75rem`, weight `600`, color `#fff`, line-height `1.15`
- Tagline: `0.875rem`, weight `400`, `rgba(255,255,255,0.6)`
- Scroll: horizontal with `scroll-snap-type: x mandatory`, gap `1.25rem`

### Project Cards
- Size: `340px × 453px`
- Border radius: `1.25rem`
- Image: `position: absolute; inset: 0; object-fit: cover`
- Frosted overlay: `backdrop-filter: blur(22px)`, `background: rgba(16,8,4,0.52)`, starts at `top: 38%`
- Overlay padding: `1.4rem 1.5rem 1.6rem`
- Sector/location: `1rem`, weight `400`, `rgba(255,255,255,0.65)`
- Title: `1.75rem`, weight `700`, letter-spacing `−0.02em`
- Button: outline style (see above), `margin-top: auto` to pin to bottom

### Service Links (non-clickable)
```
padding-top: 1.75rem
padding-bottom: 1.75rem
cursor: default (div, not <a>)
```

### Our Approach Section
- Background: full-bleed image + dark overlay `linear-gradient(135deg, rgba(5,5,5,0.92), rgba(5,5,5,0.78))`
- Inner padding: `5.5rem` top + bottom
- Pillars: 3-column grid, separated by `1px solid rgba(255,255,255,0.08)` vertical borders
- Pillar padding: `2.5rem` (between columns)
- Number: `3rem`, weight `900`, `rgba(249,115,22,0.2)`
- Pillar title: `1.15rem`, weight `700`, `#fff`
- Pillar description: `0.875rem`, `rgba(255,255,255,0.52)`, line-height `1.75`
- Heading: `3rem`, weight `800`, letter-spacing `−0.02em`
- Eyebrow chip: orange pill, `0.68rem`, weight `700`, letter-spacing `0.14em`, uppercase

### Who We Are Section
- Layout: 2-column grid `45% / 1fr`
- Image col: `border-radius: 1.25rem`
- Content col padding: `4rem 3.375rem`
- Heading: `3rem`, weight `800`, letter-spacing `−0.02em`
- Body: `0.95rem`, `rgba(255,255,255,0.55)`, line-height `1.75`, max-width `46ch`

### Footer
- Border top: `1px solid rgba(255,255,255,0.08)`
- Padding: `1.5rem 2.5rem`
- Layout: flex row, `space-between`
- Copyright: `0.8rem`, `rgba(255,255,255,0.3)`
- Email link: `0.8rem`, `rgba(255,255,255,0.4)` → hover `#f97316`

### Sector Page Footer CTA
- Border top: `1px solid rgba(255,255,255,0.08)`
- Padding: `4rem 2.5rem` (mobile: `3rem 1.25rem`)
- Title: `clamp(1.5rem → 2.25rem)`, weight `700`, letter-spacing `−0.02em`
- Subtitle: `0.95rem`, `rgba(255,255,255,0.5)`

---

## Dividers

Use `<hr>` with no border, only `border-top: 1px solid rgba(255,255,255,0.08)`. Margin matches section horizontal padding (`0 2.5rem` desktop, `0 1.25rem` mobile).

---

## Responsive Breakpoints

| Breakpoint | Width | Key changes |
|---|---|---|
| Mobile | `≤ 480px` | Single-column grids, full-width cards |
| Tablet | `≤ 767px` | Stack approach pillars, who-we-are single column |
| Desktop small | `≤ 991px` | 2-column project grid |
| Desktop | `> 991px` | Full layout |

Horizontal padding:
- Desktop: `2.5rem`
- Mobile: `1.25rem`

---

## Images

- All card images: `object-fit: cover`, full-bleed behind overlays
- Logo: `height: 44px`, `width: auto`
- Qualification badge: `height: 64px`, `border-radius: 6px`
- Hero marquee logos: `height: 3.5rem`, `filter: brightness(0) invert(1)`, `opacity: 0.75`

---

## Scrollbars (custom)

Used on sector horizontal scroll:
```css
scrollbar-width: thin;
scrollbar-color: rgba(249,115,22,0.4) rgba(255,255,255,0.05);
/* webkit */
height: 3px;
thumb: rgba(249,115,22,0.45), border-radius: 2px;
```
