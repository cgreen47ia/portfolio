# Bold Canvas

## 1. Design System Name

**Bold Canvas** — an original design system for premium creative portfolio and studio marketing surfaces. The name reflects large typographic “canvases,” confident color fields, and a gallery-like presentation rhythm inspired by high-end editorial SaaS landing pages — without copying any referenced brand identity.

## 2. Value

Bold Canvas gives designers and developers a shared language for building portfolio tools, creative agency sites, and showcase-driven products. It provides concrete tokens, component specs, and layout rules so teams can ship consistent, high-contrast marketing and app UI quickly — while maintaining accessibility and copyright-safe originality.

## 3. Intent

**Mood:** Confident, editorial, gallery-grade. Feels like walking into a well-curated design studio — loud when it needs to be, restrained everywhere else.

**Experience goals:**
- Lead with typography and color blocks, not decoration
- Create immediate hierarchy through scale and contrast
- Balance bold marketing moments with readable, functional UI
- Support dark immersive sections and bright accent fields in the same flow

**Product qualities:** Premium, direct, craft-forward, unapologetically visual.

## 4. Boundary

**Use for:**
- Creative portfolio builders and showcase platforms
- Agency and studio marketing sites
- Product landing pages with editorial hero sections
- Dashboard shells that need a bold marketing layer on top

**Do not use for:**
- Dense enterprise data applications (use a calmer system)
- Medical, legal, or compliance-heavy interfaces requiring conservative visuals
- Products targeting children or playful consumer apps

**Copyright-safe boundaries:**
- References are inspiration only; do not copy logos, exact layouts, brand-identifiable palettes, proprietary illustrations, or distinctive interaction patterns from source products.
- Do not present this system as affiliated with or derived from any referenced brand.
- Avoid eagle mascots, crown motifs, or sunburst decorative patterns from reference sites.

## 5. Visual Principles

1. **Type as architecture** — Display headlines are the primary visual element; imagery supports, never competes.
2. **Color fields, not gradients** — Sections are defined by solid background blocks (accent, dark, light) with sharp transitions between them.
3. **High contrast by default** — Pair near-black with white or saturated accent backgrounds; never rely on low-contrast gray-on-gray for primary content.
4. **Generous outer margins, tight inner grids** — Wide section padding frames content; internal columns align to a strict 12-column grid.
5. **Caps for wayfinding, title case for form fields** — Navigation and eyebrows use uppercase with tracked letter-spacing; form labels and input values use title case; body copy stays sentence case.
6. **Rounded utility, sharp structure** — Buttons and cards use consistent border-radius; layout edges and section breaks remain geometric and grid-aligned.
7. **Monochrome media, color UI** — Photography and thumbnails default to grayscale or muted treatment; UI chrome carries the accent palette.

## 6. Layout and Spacing

### Grid

- **Desktop (≥1280px):** 12 columns, 24px gutters, max content width 1440px
- **Tablet (768px–1279px):** 8 columns, 20px gutters, max width 100% with 40px horizontal padding
- **Mobile (<768px):** 4 columns, 16px gutters, 20px horizontal padding

### Containers

| Token | Value | Use |
|-------|-------|-----|
| `--container-max` | `1440px` | Page shell |
| `--container-narrow` | `960px` | Long-form text, modals |
| `--container-wide` | `100%` | Full-bleed color sections |
| `--section-padding-x` | `clamp(20px, 5vw, 80px)` | Horizontal section inset |
| `--section-padding-y` | `clamp(64px, 10vw, 160px)` | Vertical section rhythm |

### Spacing scale

| Token | Value |
|-------|-------|
| `--space-1` | `4px` |
| `--space-2` | `8px` |
| `--space-3` | `12px` |
| `--space-4` | `16px` |
| `--space-5` | `24px` |
| `--space-6` | `32px` |
| `--space-7` | `48px` |
| `--space-8` | `64px` |
| `--space-9` | `96px` |
| `--space-10` | `128px` |
| `--space-11` | `160px` |
| `--space-12` | `192px` |

### Vertical rhythm

- Stack gap (related items): `--space-4` to `--space-5`
- Component groups: `--space-6`
- Section header to content: `--space-7`
- Between major sections: `--space-9` (within same background) or full background swap (no extra gap)

### Responsive behavior

- Display headings scale down ~35% on tablet, ~50% on mobile using `clamp()`
- Multi-column hero footers collapse to single column on mobile
- Navigation condenses to logo + menu trigger below 768px
- Tables scroll horizontally inside a bordered container on mobile

## 7. Color System

### Base tokens

| Token | Value | Role |
|-------|-------|------|
| `--color-accent` | `#FFC940` | Primary brand field (hero blocks, highlights) |
| `--color-accent-deep` | `#E8A800` | Hover on accent surfaces, darker accent UI |
| `--color-blue` | `#2A5F9E` | Secondary brand accent (links, highlights, cool contrast on dark) |
| `--color-blue-deep` | `#1E4578` | Blue hover/active, pressed states |
| `--color-blue-bg` | `#E6EEF6` | Subtle blue tint for badges, tags, and tinted surfaces |
| `--color-cta` | `#C4451E` | Primary call-to-action buttons |
| `--color-cta-hover` | `#A83818` | CTA hover/active |
| `--color-ink` | `#0A0A0A` | Primary text on light/accent backgrounds |
| `--color-ink-inverse` | `#FAFAFA` | Primary text on dark backgrounds |
| `--color-canvas` | `#FAFAFA` | Default page background |
| `--color-surface` | `#FFFFFF` | Cards, nav bar, raised panels |
| `--color-surface-muted` | `#EBEBEB` | Secondary section backgrounds |
| `--color-surface-dark` | `#141414` | Immersive hero / feature sections |
| `--color-surface-raised` | `#1F1F1F` | Elevated panels on dark backgrounds |
| `--color-border` | `#D4D4D4` | Default borders, dividers |
| `--color-border-strong` | `#0A0A0A` | Emphasis borders, ghost buttons on light |
| `--color-border-inverse` | `#FAFAFA` | Ghost buttons on dark/accent |
| `--color-text-secondary` | `#525252` | Supporting body text on light |
| `--color-text-muted` | `#737373` | Captions, placeholders |
| `--color-text-secondary-inverse` | `#A3A3A3` | Supporting text on dark |
| `--color-success` | `#15803D` | Success states |
| `--color-success-bg` | `#DCFCE7` | Success alert background |
| `--color-warning` | `#B45309` | Warning states |
| `--color-warning-bg` | `#FEF3C7` | Warning alert background |
| `--color-error` | `#B91C1C` | Error states |
| `--color-error-bg` | `#FEE2E2` | Error alert background |
| `--color-info` | `#1D4ED8` | Info states |
| `--color-info-bg` | `#DBEAFE` | Info alert background |
| `--color-overlay` | `rgba(10, 10, 10, 0.6)` | Modal backdrop |
| `--color-focus-ring` | `#C4451E` | Keyboard focus outline |

### Semantic roles

- **Background:** `--color-canvas` (default), `--color-accent` (marketing blocks), `--color-surface-dark` (immersive)
- **Surface:** `--color-surface`, `--color-surface-muted`, `--color-surface-raised`
- **Border:** `--color-border` (subtle), `--color-border-strong` (emphasis)
- **Text-primary:** `--color-ink` or `--color-ink-inverse` depending on surface
- **Text-secondary / muted:** paired inverse variants per background
- **Accent:** `--color-accent` for fields and secondary CTAs; `--color-cta` for primary actions; `--color-blue` for links, informational highlights, and cool contrast on dark surfaces

### States

| State | Rule |
|-------|------|
| Hover | Darken fills 8–12%; underline text links |
| Active | Darken fills 15%; scale buttons to `0.98` |
| Focus (general UI) | `2px solid --color-focus-ring`, `2px offset` |
| Focus (form fields) | Border `--color-blue`, `2px` ring `rgba(42, 95, 158, 0.2)`; error fields keep `--color-error` |
| Disabled | `opacity: 0.45`, no pointer events |
| Selected | `--color-ink` background with `--color-ink-inverse` text (tabs, tags) |

### Accessibility

- Body text on `--color-canvas` / `--color-surface`: `--color-ink` → **15.8:1** (AAA)
- Body text on `--color-accent`: `--color-ink` → **≥8:1** (AAA)
- CTA button: white text on `--color-cta` → **≥4.5:1** (AA)
- `--color-blue` on `--color-surface`: **≥4.5:1** (AA) for UI text and links
- Secondary text `--color-text-secondary` on white → **≥4.5:1** (AA)
- Never use `--color-text-muted` for essential instructions alone; pair with icon or label
- Focus rings must remain visible on all background variants

## 8. Typography

### Font stack

- **Display / UI sans:** `"DM Sans", "Helvetica Neue", Arial, sans-serif`
- **Editorial serif (optional display):** `"Libre Baskerville", Georgia, serif`
- **Monospace:** `"JetBrains Mono", "Consolas", monospace`

Load via Google Fonts: DM Sans (400, 500, 700), Libre Baskerville (400, 700).

### Type scale

| Token | Size | Weight | Line height | Use |
|-------|------|--------|-------------|-----|
| `--text-display-xl` | `clamp(2.75rem, 6vw, 5.5rem)` | 700 | 1.05 | Hero headlines |
| `--text-display-lg` | `clamp(2.25rem, 4.5vw, 4rem)` | 700 | 1.08 | Section headlines |
| `--text-display-md` | `clamp(1.75rem, 3vw, 2.75rem)` | 700 | 1.12 | Feature titles |
| `--text-heading-lg` | `2rem` | 700 | 1.2 | Page titles |
| `--text-heading-md` | `1.5rem` | 700 | 1.25 | Card titles |
| `--text-heading-sm` | `1.125rem` | 700 | 1.3 | Subsections |
| `--text-body-lg` | `1.125rem` | 400 | 1.6 | Lead paragraphs |
| `--text-body-md` | `1rem` | 400 | 1.6 | Default body |
| `--text-body-sm` | `0.875rem` | 400 | 1.5 | Secondary body |
| `--text-label` | `0.75rem` | 500 | 1.2 | Eyebrows, nav, badges |
| `--text-caption` | `0.6875rem` | 400 | 1.4 | Fine print |

### Headings, body, labels, captions

- **Display headings:** DM Sans 700, `letter-spacing: -0.02em`, tight line-height
- **Editorial accent headings:** Libre Baskerville 400/700 for featured callouts only (max one per section)
- **Body:** DM Sans 400, max width 65ch for readability
- **Form field labels:** DM Sans 500, title case (`text-transform: capitalize`), `--text-body-sm`, `letter-spacing: 0`
- **Nav / eyebrows:** DM Sans 500, uppercase, `letter-spacing: 0.12em`, `--text-label`
- **Form inputs:** DM Sans 400, title case (`text-transform: capitalize`), `--text-body-md`
- **Numeric / code:** JetBrains Mono for tables, IDs, timestamps

## 9. Components

### Buttons

**Anatomy:** Label, optional trailing arrow icon (Lucide `arrow-right`), min-height 44px.

| Variant | Background | Text | Border |
|---------|------------|------|--------|
| Primary | `--color-cta` | white | none |
| Secondary | `--color-accent` | `--color-ink` | none |
| Ghost (light) | transparent | `--color-ink` | `1px --color-border-strong` |
| Ghost (dark) | transparent | `--color-ink-inverse` | `1px --color-border-inverse` |
| Pill | same as above | same | `border-radius: 999px` |

**Sizes:** sm (36px), md (44px), lg (52px). Padding: sm `12px 20px`, md `14px 28px`, lg `18px 36px`.

**States:** Hover darkens fill; focus ring; disabled opacity 0.45.

### Cards

**Anatomy:** Optional eyebrow, title, body, footer actions.

| Variant | Background | Border | Shadow |
|---------|------------|--------|--------|
| Default | `--color-surface` | `1px --color-border` | none |
| Elevated | `--color-surface` | none | `--shadow-md` |
| Interactive | `--color-surface` | `1px --color-border` | hover `--shadow-lg`, translateY -2px |
| Dark feature | `--color-surface-dark` | none | none, 20px radius |

Padding: `--space-6`. Radius: `--radius-lg` (16px). Light-surface cards (`Default`, `Elevated`, `Interactive`) always use `--color-ink` titles and `--color-text-secondary` body — never inherit inverse text from dark page sections (`.theme-dark`).

**Dark feature card:** `--color-surface-dark` background, `--color-ink-inverse` text, `--radius-xl`.

### Forms

**Labels:** Title case (`text-transform: capitalize`), DM Sans 500, `--text-body-sm` (0.875rem), `letter-spacing: 0`, `5px` margin below label (3px tighter than `--space-2`).

**Hints:** Optional helper below control. Class: `.field-hint`. Same size as labels/errors (`--text-body-sm`), `5px` margin above, `--color-text-muted`. Linked via `aria-describedby`.

**Inputs:** 44px height, `1px --color-border`, `--radius-md` (8px), padding `--space-4`, `text-transform: capitalize` (title case for entered and placeholder text). Focus: border `--color-blue`, `2px` ring `rgba(42, 95, 158, 0.2)`. Error fields retain `--color-error` border and ring on focus.

**Select:** Custom combobox pattern (native `<select>` menus cannot be styled consistently). Trigger matches input dimensions and title-case text. Lucide `chevron-down` at 20px on the right; rotates 180° when open. Focus/open: `--color-blue` border and ring (matches inputs). Menu panel: flush below trigger, shared `--color-blue` border when open, `--shadow-md`, bottom radius only. Options: `--space-3` / `--space-4` padding; hover `--color-surface-muted`; selected `--color-cta` background with white text. Error state: `--color-error` border; open menu keeps error border/ring.

**Checkbox:** 20×20px, 2px border, checked fill `--color-cta`. Checkbox labels use sentence case (not title case).

**Validation:** Error border `--color-error`. Hint and error text: `--text-body-sm`, `5px` margin above (tight to control). Hints use `--color-text-muted`. Errors use flex layout with Lucide `circle-alert` icon (16px, `2px` top offset for optical alignment) left of message, `--color-error` text, `role="alert"`, linked via `aria-describedby`.

### Navigation

**Top bar:** Fixed or sticky, `--color-surface` background, `--shadow-sm`, height 64px, horizontal padding `--section-padding-x`.

**Links:** Uppercase label style, `--space-5` gap, hover underline.

**Mobile:** Hamburger trigger, full-screen overlay `--color-surface-dark` with inverse links.

**Badge on link:** Small pill `--color-cta` background, white `--text-caption` uppercase.

### Tabs

Underline-style on light backgrounds: inactive `--color-text-muted`, active `--color-ink` with 2px bottom border `--color-cta`. Padding `--space-4` horizontal.

### Modals / dialogs

Centered panel, `--container-narrow` max-width, `--radius-lg`, `--shadow-xl`, padding `--space-6`. Backdrop `--color-overlay`. Close button top-right, 44×44px target.

### Tables

Header row: uppercase `--text-label`, border-bottom `2px --color-border-strong`. Row height 52px, zebra optional with `--color-surface-muted` at 50% opacity. Cell padding `--space-4`.

### Badges

Pill shape, padding `4px 10px`, `--text-caption` uppercase. Text and background use paired semantic tokens — never inherit section text color (e.g. on `.theme-dark` surfaces).
- **New (`badge--cta`):** `--color-cta` bg, white text
- **Neutral (`badge--neutral`):** `--color-surface-muted` bg, `--color-ink`
- **Success / Warning / Error:** matching `--color-*-bg` / `--color-*` text pairs

### Alerts

Full-width or inline banner, left accent border 4px, padding `--space-4` `--space-5`, `--radius-md`, vertical stack with `--space-1` gap.

**Anatomy:**
- **Title row (`.alert__title-row`):** flex, `align-items: center`, `--space-4` gap. Lucide icon 20px (`.alert__icon`) vertically centered with bold title (`strong`, `--text-body-sm`, line-height 1.5).
- **Message (`.alert__message`):** `--text-body-sm`, line-height 1.5, indented `calc(20px + var(--space-4))` to align with title text (not icon).

**Variants** — text and icons use semantic token on matching bg; never inherit `.theme-dark` inverse text:
| Variant | Background | Border / text |
|---------|------------|---------------|
| Success | `--color-success-bg` | `--color-success` |
| Warning | `--color-warning-bg` | `--color-warning` |
| Error | `--color-error-bg` | `--color-error` |
| Info | `--color-blue-bg` | border `--color-blue`, text `--color-blue-deep` |

### Tooltips

Dark tooltip: `--color-surface-dark` bg, `--color-ink-inverse` text, `--text-body-sm`, padding `6px 10px`, `--radius-sm`, max-width 240px.

### Empty states

Centered layout, Lucide icon 48px `--color-text-muted`, heading `--text-heading-sm`, body `--text-body-sm`, primary action button below. Optional illustration placeholder area 240×160px with dashed border.

### Loading states

**Spinner:** 24px circle, 2px stroke `--color-cta`, rotating border-top transparent.

**Skeleton:** `--color-surface-muted` blocks with subtle pulse animation, `--radius-md`.

### Error states

**Inline (form):** Red border on field + `.field-error` message with `circle-alert` icon.

**Banner:** Reuse alert anatomy (`.alert--error`); same title-row + message layout as other alerts.

## 10. Effects and Surface Treatment

### Shadows

| Token | Value |
|-------|-------|
| `--shadow-sm` | `0 1px 3px rgba(10, 10, 10, 0.08)` |
| `--shadow-md` | `0 4px 12px rgba(10, 10, 10, 0.1)` |
| `--shadow-lg` | `0 12px 32px rgba(10, 10, 10, 0.12)` |
| `--shadow-xl` | `0 24px 48px rgba(10, 10, 10, 0.16)` |

### Borders

- Hairline: `1px solid var(--color-border)`
- Strong divider: `1px solid var(--color-ink)` or full-width on accent sections
- Eyebrow line: 48px × 1px `--color-border-inverse` beside label text

### Gradients

None for primary surfaces. Optional subtle dark overlay on hero photography: `linear-gradient(to top, rgba(10,10,10,0.7), transparent)`.

### Blur and opacity

- Modal backdrop: 60% opacity, no blur (keep performance simple)
- Logo strip: `opacity: 0.45` on monochrome marks
- Disabled elements: `opacity: 0.45`

### Border radius

| Token | Value | Demo / use |
|-------|-------|------------|
| `--radius-sm` | `4px` | Small controls |
| `--radius-md` | `8px` | Inputs, alerts |
| `--radius-lg` | `16px` | Cards |
| `--radius-xl` | `24px` | Dark feature cards |
| `--radius-full` | `999px` | Pills, badges |

Radius previews use `--color-accent` background with `--color-ink` labels (readable contrast). Do not use `--color-cta` as demo fill — insufficient contrast with dark text.

### Depth / elevation

- Level 0: flat color fields
- Level 1: cards, nav bar (`--shadow-sm`)
- Level 2: dropdowns, interactive cards (`--shadow-md`)
- Level 3: modals (`--shadow-xl`)

## 11. Motion and Interaction

| Token | Value |
|-------|-------|
| `--duration-fast` | `120ms` |
| `--duration-normal` | `200ms` |
| `--duration-slow` | `320ms` |
| `--ease-out` | `cubic-bezier(0.22, 1, 0.36, 1)` |
| `--ease-in-out` | `cubic-bezier(0.65, 0, 0.35, 1)` |

- Hover transitions: color/background/box-shadow over `--duration-normal`
- Button active: scale `0.98` over `--duration-fast`
- Interactive cards: hover `--shadow-lg`, `translateY(-2px)` over `--duration-normal`
- **Motion demo card (`.motion-card`):** light `--color-surface` on dark sections; `--color-ink` title, `--color-text-secondary` body; hover `--shadow-lg`, `translateY(-4px)`, border `--color-accent-deep`
- Modal enter: fade backdrop + translate panel 8px up
- Skeleton pulse: 1.5s infinite, subtle opacity oscillation
- **Reduced motion:** `@media (prefers-reduced-motion: reduce)` — disable transforms and set all durations to 0.01ms

## 12. Iconography and Imagery

### Icons

- **Library:** Lucide (outline), default stroke width 1.75px
- **Sizes:** sm 16px, md 20px, lg 24px, xl 48px (empty states)
- **Color:** inherit text color; on buttons match button text color

### Imagery

- **Ratios:** Hero 16:9, portrait grid 3:4, card thumbnails 4:3
- **Treatment:** Desaturate to 100% for portrait grids; optional `--color-overlay` on hero photos
- **Placeholders:** `--color-surface-muted` with centered caption; dashed `2px --color-border`
- **Source:** Unsplash for stock when available; alt text required

## 13. Accessibility Guidelines

- Minimum contrast WCAG AA (4.5:1 body, 3:1 large text); prefer AAA for primary pairings
- Visible focus: general UI uses 2px `--color-focus-ring` outline; form fields use `--color-blue` border + ring
- Light-surface components (cards, badges, alerts, motion cards) on `.theme-dark` sections must set explicit text colors — do not inherit `--color-ink-inverse`
- All interactive targets ≥ 44×44px
- Semantic HTML: `header`, `nav`, `main`, `section`, `button`, `table`, `dialog`
- Form fields require visible labels; errors linked via `aria-describedby`
- Modals trap focus, close on Escape, restore focus on close
- Respect `prefers-reduced-motion`
- Do not convey status by color alone — pair with icon or text

## 14. Implementation Notes

### CSS variables

Group tokens on `:root`:

```css
/* Color */
--color-accent, --color-blue, --color-cta, --color-ink, …

/* Typography */
--text-display-xl, --font-sans, --font-serif, …

/* Space */
--space-1 … --space-12

/* Radius, shadow, motion */
--radius-md, --shadow-md, --duration-normal, …
```

### Design tokens

- Theme by setting surface context classes: `.theme-light`, `.theme-dark`, `.theme-accent`
- `.theme-dark` sets `--color-ink-inverse` for section headings and descriptions only
- Components with their own background must opt out of inherited section text color:
  - **Badges / alerts:** semantic `--color-*` text on `--color-*-bg` (or `--color-blue-bg` for info)
  - **Light cards / motion cards:** `--color-ink` titles, `--color-text-secondary` body
  - **Dark feature cards (`.card-dark`):** `--color-ink-inverse` text
- Extend by adding semantic aliases (e.g., `--color-brand`) that reference base tokens

### Reusable patterns

- `.section` — horizontal/vertical padding tokens
- `.container` — max-width centered shell
- `.eyebrow` — label + optional line
- `.display-headline` — display-xl typography
- `.btn`, `.btn--primary`, `.btn--ghost` — button variants
- `.card`, `.card--elevated`, `.card-dark` — card variants
- `.field`, `.field-hint`, `.field-error`, `.select`, `.select-trigger` — form controls
- `.alert`, `.alert__title-row`, `.alert__message` — alert anatomy
- `.grid-12` — CSS grid with responsive column collapse

### Responsive behavior

- Mobile-first base styles; enhance at 768px and 1280px
- Use `clamp()` for fluid display type
- Collapse multi-column marketing layouts to single column below 768px
- Navigation switches to overlay menu below 768px
