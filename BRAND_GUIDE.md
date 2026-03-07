# Faisca Brand Guide

## Brand Architecture

| Aspect | Faisca | Presa |
|--------|--------|-------|
| **Type** | Company | Product |
| **Domain** | faisca.dev | presa.dev |
| **Color** | Orange — `oklch(0.70 0.18 55)` / `#f07900` | Indigo — `oklch(0.50 0.20 280)` / `#5449d0` |
| **Tagline** | "For those who build their own fire" | "HTML to PDF in one API call" |
| **Voice** | Builder-to-builder, warm, opinionated | Direct, cool, professional |
| **Logo** | "faísca." wordmark with orange dot | Press mark (P in rounded square) |

### Connection Rules

- Presa leads all product surfaces (dashboard, docs, presa.dev, marketplace)
- Faisca appears as **"A Faisca project"** in footers only — never in headers, hero sections, or primary CTAs
- Connection is structural (footer link, org name), not verbal
- Never mix voices between Faisca and Presa surfaces

---

## Logo Usage

### Presa Press Mark

Bold geometric "P" letterform inside a rounded square, evoking a printing press stamp. Adapts between light and dark modes automatically via CSS media query.

| Variant | File | Usage |
|---------|------|-------|
| Icon (adaptive) | `shared/brand/presa-icon.svg` | Favicon, marketplace icon, small contexts |
| Full logo (light) | `shared/brand/presa-logo.svg` | Headers, hero sections on light backgrounds |
| Full logo (dark) | `shared/brand/presa-logo-dark.svg` | Headers, hero sections on dark backgrounds |
| PNG rasters | `shared/brand/presa-icon-{48,96,256,512}.png` | Marketplace listings, social media |

**Requirements:**
- Minimum size: 16x16px (icon variant)
- Clear space: 25% of mark width on all sides
- Never stretch, rotate, recolor, add effects, or place on busy backgrounds

### Faisca Wordmark

"faísca." wordmark with orange dot accent.

| Variant | File | Usage |
|---------|------|-------|
| Light mode | `shared/brand/faisca-logo.svg` | faisca.dev, light backgrounds |
| Dark mode | `shared/brand/faisca-logo-dark.svg` | Dark backgrounds |

---

## Color Palette

### Presa — Indigo Scale (OKLch Hue 280)

| Token | OKLch | Hex | Usage |
|-------|-------|-----|-------|
| `--presa-50` | `oklch(0.97 0.02 280)` | `#f2f4ff` | Tint backgrounds |
| `--presa-100` | `oklch(0.93 0.04 280)` | `#e2e6ff` | Hover tints |
| `--presa-200` | `oklch(0.87 0.08 280)` | `#c9cfff` | Subtle borders |
| `--presa-300` | `oklch(0.77 0.12 280)` | `#a5abff` | Muted accents |
| `--presa-400` | `oklch(0.68 0.17 280)` | `#8688fe` | Dark mode accent |
| `--presa-500` | `oklch(0.50 0.20 280)` | `#5449d0` | **Light mode accent (base)** |
| `--presa-600` | `oklch(0.44 0.20 280)` | `#4635bc` | Hover on base |
| `--presa-700` | `oklch(0.37 0.17 280)` | `#352795` | Active on base |
| `--presa-800` | `oklch(0.30 0.13 280)` | `#261d6c` | Deep accent |
| `--presa-900` | `oklch(0.24 0.09 280)` | `#191648` | Near-black indigo |
| `--presa-950` | `oklch(0.18 0.06 280)` | `#0d0c2b` | Darkest indigo |

### Faisca — Orange Scale (OKLch Hue 55)

| Token | OKLch | Hex | Usage |
|-------|-------|-----|-------|
| `--faisca-400` | `oklch(0.78 0.15 55)` | `#ff9b50` | Light variant |
| `--faisca-500` | `oklch(0.70 0.18 55)` | `#f07900` | **Base orange** |
| `--faisca-600` | `oklch(0.62 0.18 55)` | `#d46000` | Dark variant |

### Contrast Ratios (WCAG AA)

- Presa 500 on white: 6.48:1
- Presa 400 on dark bg: 5.65:1

---

## Typography

**Font family: Geist** — used across all surfaces.

| Font | Weight | Usage |
|------|--------|-------|
| Geist Sans 400 | Regular | Body text, descriptions |
| Geist Sans 500 | Medium | Labels, navigation |
| Geist Sans 600 | Semibold | Headings, emphasis |
| Geist Sans 700 | Bold | Hero text, strong headings |
| Geist Mono 400 | Regular | Code blocks, API references, technical values |

Fallback stack: `ui-sans-serif, system-ui, sans-serif`.

---

## Tone & Voice

### 5 Core Principles

1. **Direct.** Say what it does. Skip the preamble.
2. **Code-first.** Show the code before describing it.
3. **Confident, not loud.** No superlatives ("blazing fast", "revolutionary").
4. **Diagnostic.** Error messages explain what broke and how to fix it.
5. **LLM-friendly.** Documentation is structured and explicit — the primary reader may be a coding agent.

### Voice by Surface

| Surface | Voice | Style |
|---------|-------|-------|
| Documentation | Presa | Instructional, zero fluff |
| Dashboard | Presa | Minimal, functional labels |
| Error messages | Presa | Diagnostic + actionable |
| presa.dev | Presa | Confident, code-forward |
| faisca.dev | Faisca | Philosophical, portfolio-focused |
| Marketplace listing | Presa | Short description + features + "Free tier included" |
| GitHub READMEs | Presa | Technical, direct (Faisca tone for org profile only) |

### Avoid

- "We're excited to announce"
- "Powerful", "seamless", "cutting-edge"
- Hedging: "might", "should", "try to"
- Faisca voice on Presa surfaces (and vice versa)

---

## Design Tokens

Canonical source: [`shared/tokens.css`](https://github.com/faiscadev/presa/blob/main/shared/tokens.css) in the Presa repository.
