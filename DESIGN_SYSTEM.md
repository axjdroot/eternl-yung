# DESIGN SYSTEM

**Brand**: AWKWRDx Reference Theme
**Aesthetic**: Minimal Streetwear, Dark Base, Category-First Browsing, Space & Discipline.
**Audience**: Modern Pakistan, local audience, streetwear drop culture.

## Typography

### PRIMARY DISPLAY — Pikabu
- **Use**: Brand logo text, hero headlines, drop titles, section statement text
- **Font**: Local Asset (Pikabu.ttf)
- **Weight**: Normal (Distinctive streetwear style)
- **Fallback**: Syne, sans-serif
- **Rendering**: `font-display: swap; -webkit-font-smoothing: antialiased;`

### SECONDARY HEADING — Space Grotesk
- **Use**: Collection names, category headers, product names in catalog, labels, eyebrows
- **Weight**: 600
- **Transform**: Uppercase
- **Letter Spacing**: `0.05em`

### BODY / UI — Coolvetica
- **Use**: Product descriptions, cart line items, UI copy, navigation links, footer
- **Font**: Local Asset (Coolvetica.otf)
- **Weight**: Normal
- **Size**: 15px base
- **Line Height**: 1.6
- **Letter Spacing**: `0.01em`

### LABEL / MONO — Space Mono
- **Use**: Price display, stock badges, drop labels, SKUs, sizes
- **Weight**: 400
- **Transform**: Uppercase
- **Letter Spacing**: `0.10em` minimum

## Color System

**CSS Custom Properties Pattern**: Must define `--color-bg`, `--color-text`, `--color-muted`, `--color-border`, `--color-surface` per scheme.

#### VOID (Primary Default)
- `--color-bg`: `#0D0D0D`
- `--color-text`: `#EFEFEB`
- `--color-muted`: `#5A5A55`
- `--color-border`: `#1E1E1A`
- `--color-surface`: `#161616`

#### CHALK (Product Cards / Clean Sections)
- `--color-bg`: `#F4F1EC`
- `--color-text`: `#0D0D0D`
- `--color-muted`: `#9A9690`
- `--color-border`: `#E2DFD9`
- `--color-surface`: `#EDEAE4`

#### ACCENT (CTAs, Sales, Drops)
- `--color-bg`: `#388D73` (Eternl Green)
- `--color-text`: `#0D0D0D`
- `--color-muted`: `#3A4A00`
- `--color-border`: `#0D0D0D`

#### GHOST (Editorial Blocks, Lookbooks)
- `--color-bg`: `#131313`
- `--color-text`: `#7A7A75`
- `--color-muted`: `#3A3A35`
- `--color-border`: `#222220`
- `--color-surface`: `#1A1A18`

> **ETERNL GREEN RULE**: `#388D73` appears *only* on announcement bar bg, primary "Add to Cart" bg, "SALE"/Drop badge bg, active filter pills, and scroll progress bar. Never as section background or on text unless dark background.

## Spacing & Layout Tokens

- `--sp-1`: `4px`
- `--sp-2`: `8px`
- `--sp-3`: `12px`
- `--sp-4`: `16px`
- `--sp-6`: `24px`
- `--sp-8`: `32px`
- `--sp-12`: `48px`
- `--sp-16`: `64px`
- `--sp-24`: `96px`
- `--sp-32`: `128px`

- `--gap-grid`: `2px`
- `--gap-section`: `1px`
- `--pad-section`: `72px`
- `--pad-section-m`: `40px`
- `--max-width`: `1440px`
- `--max-narrow`: `900px`

- `--radius`: `0px` (Exception: color swatch circles `50%`)

## Motion & Interaction

- `--ease-out`: `cubic-bezier(0.16, 1, 0.3, 1)`
- `--ease-in`: `cubic-bezier(0.7, 0, 0.84, 0)`
- `--dur-fast`: `120ms`
- `--dur-base`: `220ms`
- `--dur-slow`: `380ms`

**Principles**:
- Reveal on scroll: `fade + translateY(12px) → visible`
- Image hover: crossfades `200ms ease`
- Button states: bg color transitions only `120ms`
- **Prefers Reduced Motion**: Skip all transforms/transitions immediately. Non-negotiable. 
- Focus visible outline: `2px solid #388D73`, offset `2px`.

## Class Prefixes & Naming
- All section-specific and custom CSS classes prefixed with `.sw-` to prevent future conflicts.
- Adhere strictly to BEM methodologies.
- Use mobile-first approach.
