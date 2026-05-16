---
name: Lutof
description: The fastest way to preview, compare, and manage your color grading library.
colors:
  background: "oklch(0.141 0.005 285.823)"
  foreground: "oklch(0.985 0 0)"
  primary: "oklch(0.92 0.004 286.32)"
  primary-foreground: "oklch(0.21 0.006 285.885)"
  muted: "oklch(0.274 0.006 286.033)"
  muted-foreground: "oklch(0.705 0.015 286.067)"
  destructive: "oklch(0.704 0.191 22.216)"
  border: "oklch(1 0 0 / 10%)"
  ring: "oklch(0.552 0.016 285.938)"
  amber: "oklch(0.75 0.15 45deg)"
  amber-foreground: "oklch(0.15 0.02 45deg)"
typography:
  display:
    fontFamily: "'Outfit Variable', sans-serif"
    fontSize: "clamp(3rem, 8vw, 4.5rem)"
    fontWeight: 700
    lineHeight: 0.95
    letterSpacing: "-0.03em"
  headline:
    fontFamily: "'Outfit Variable', sans-serif"
    fontSize: "1.875rem"
    fontWeight: 700
    lineHeight: 1.1
    letterSpacing: "-0.03em"
  title:
    fontFamily: "'Outfit Variable', sans-serif"
    fontSize: "1.5rem"
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: "-0.03em"
  body:
    fontFamily: "'Outfit Variable', sans-serif"
    fontSize: "1rem"
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: "normal"
  label:
    fontFamily: "'Outfit Variable', sans-serif"
    fontSize: "0.875rem"
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: "normal"
rounded:
  sm: "0.375rem"
  md: "0.5rem"
  lg: "0.625rem"
  xl: "0.875rem"
  2xl: "1.125rem"
  3xl: "1.375rem"
  4xl: "1.625rem"
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.primary-foreground}"
    rounded: "{rounded.lg}"
    padding: "0px 32px"
    height: "48px"
    typography: "{typography.label}"
  demo-container:
    backgroundColor: "{colors.muted}"
    textColor: "{colors.muted-foreground}"
    rounded: "{rounded.lg}"
    size: "aspect-ratio: 16/9"
---

# Design System: Lutof

## 1. Overview

**Creative North Star: "The Dark Edit Bay"**

This system is built for professionals who spend hours in dim rooms staring at calibrated monitors. Every decision assumes a low-ambient-light environment where contrast fatigue is real and color accuracy matters. The interface is dark by default, not as an aesthetic choice, but because that is where the user lives.

The visual language is deliberately restrained. There is one typeface, one weight variable, and near-zero chroma across the neutral palette. The only warmth comes from a reserved amber token that is currently held in reserve for future product UI moments. On the marketing surface, the palette is almost entirely cool zinc: slightly cold, technical, and invisible when it needs to be.

The system explicitly rejects generic SaaS landing-page theatrics: no hero metrics, no gradient text, no identical feature-card grids, no glassmorphism, no neon accents. What remains is structure, hierarchy, and speed.

**Key Characteristics:**
- Single-font system (Outfit Variable, 100–900) with weight-based hierarchy
- OKLCH color space throughout; neutrals tinted toward a cool 285° hue
- Dark-mode-first with a functional light-mode fallback
- Tactile and confident component feedback (hover scale, active press)
- Flat surfaces at rest; depth conveyed through tonal layering, not decorative shadows
- No cards as containers; content sits directly on the background surface

## 2. Colors

The palette is a near-monochrome zinc system with a single warm accent held in reserve. Every neutral is tinted toward a cool 285° hue at very low chroma (0.005–0.016), preventing the sterility of pure gray while staying invisible.

### Primary
- **Cool Zinc Light** (oklch(0.92 0.004 286.32)): The main actionable color in dark mode. Used for primary buttons, positive framing ("The Lutof Way"), and high-priority interactive elements. In light mode, this role inverts to the dark zinc below.
- **Cool Zinc Dark** (oklch(0.21 0.006 285.885)): The primary color in light mode. Dark enough for strong contrast on white backgrounds, cool enough to avoid generic black.

### Neutral
- **Deep Edit Bay** (oklch(0.141 0.005 285.823)): The dark-mode background. Deep, near-black with a subtle cool tint. This is the default surface.
- **Clean White** (oklch(1 0 0)): The light-mode background. Pure white is permitted here because the light mode is secondary; the dark surface is the identity.
- **Soft Zinc** (oklch(0.985 0 0)): Dark-mode foreground text. Nearly white, slightly muted to reduce eye strain in dim environments.
- **Panel Zinc** (oklch(0.274 0.006 286.033)): Elevated surface color in dark mode (cards, popovers, elevated containers). One step above the background.
- **Dim Zinc** (oklch(0.705 0.015 286.067)): Secondary text, placeholders, metadata. Readable but de-emphasized.
- **Border Zinc** (oklch(1 0 0 / 10%)): Subtle dividers in dark mode. Nearly invisible until needed.

### Accent
- **Warm Amber** (oklch(0.75 0.15 45deg)): A single warm accent reserved for future product UI use (warnings, progress indicators, highlights). Currently unused on the marketing surface; its rarity is intentional.
- **Amber Ink** (oklch(0.15 0.02 45deg)): Text color when amber is used as a background.

### State
- **Calibrated Red** (oklch(0.704 0.191 22.216)): Destructive actions and negative framing ("The Old Way"). A precise, non-cartoonish red that signals without shouting.

### Named Rules
**The One Voice Rule.** The primary accent (zinc light) is used on ≤15% of any given screen. Its rarity is the point. The surface is the design.

**The No-Pure-Black Rule.** Backgrounds and foregrounds are never #000 or #fff. Every neutral carries a faint cool tint (chroma 0.005–0.016) to keep the eye comfortable across long sessions.

## 3. Typography

**Display & Body Font:** Outfit Variable (100–900), with system-ui fallback
**Label/Mono Font:** Outfit Variable (same family, distinct weight)

**Character:** A geometric-humanist hybrid with generous x-height and clean curves. At display sizes it feels precise and modern; at body sizes it remains highly legible. The single-family approach keeps the system ruthlessly simple. One font, many weights.

### Hierarchy
- **Display** (700, clamp(3rem, 8vw, 4.5rem), line-height 0.95, letter-spacing -0.03em): Hero headlines only. Tight leading and aggressive tracking create impact at large sizes. Never used below the fold.
- **Headline** (700, 1.875rem / 30px, line-height 1.1, letter-spacing -0.03em): Section headings (CTA, Features). Same tracking as display, scaled down.
- **Title** (600, 1.5rem / 24px, line-height 1.2, letter-spacing -0.03em): Subsection headings, feature names. Slightly lighter weight than headlines to preserve hierarchy.
- **Body** (400, 1rem / 16px, line-height 1.6): All body text and descriptions. Comfortable for short-to-medium passages. Max line length 65ch where possible.
- **Label** (600, 0.875rem / 14px, line-height 1.4): Buttons, small headings, metadata. Semibold weight creates clear affordance at small sizes.

### Named Rules
**The Scale-Not-Size Rule.** Hierarchy is built through weight contrast and tracking, not just font-size jumps. A Title at 1.5rem/600 sits clearly below a Headline at 1.875rem/700 because the weight AND size shift together.

**The Tight-Tracking Rule.** Letter-spacing of -0.03em is reserved for Display, Headline, and Title sizes only. Body and Label use default spacing. Never apply negative tracking to body text; it degrades readability.

## 4. Elevation

This system is flat by default. Depth is conveyed through tonal contrast between background layers, not through drop shadows. Shadows appear only as transient responses to state (hover, focus, active), never as permanent structural elements.

### Shadow Vocabulary
- **Ambient Hover Glow** (`box-shadow: 0 0 20px {colors.primary} / 20%`): Applied to primary buttons on hover. A diffuse, soft glow that suggests lift without casting a directional shadow. Used sparingly; only on the primary CTA.

### Named Rules
**The Flat-By-Default Rule.** Surfaces are flat at rest. The background is the background. Elevated surfaces use a slightly lighter or darker tonal value (Panel Zinc), not a shadow. Shadows are reserved for interactive feedback.

## 5. Components

### Buttons
- **Shape:** Rounded rectangle with 10px radius (rounded-lg)
- **Primary:** Background Cool Zinc Light, text Cool Zinc Dark, height 48px, horizontal padding 32px. Semibold 14px label. Full-width on mobile; min-width 200px on desktop.
- **Hover / Focus:** Scale to 102% with a subtle ambient glow shadow. Transition: all 200ms ease-out. Focus: 2px ring in Ring Zinc with 2px offset.
- **Active:** Scale to 98%. Immediate tactile feedback.
- **Ghost / Secondary:** Not currently used on the marketing surface. When needed, use a transparent background with a 1px Border Zinc border.

### Demo Containers
- **Corner Style:** 10px radius (rounded-lg)
- **Background:** Panel Zinc at 10% opacity (`bg-muted/10`)
- **Border:** 1px Border Zinc at 30% opacity (`border-border/30`)
- **Shadow Strategy:** None at rest
- **Hover:** Border opacity increases to 30% toward primary (`hover:border-primary/30`). A quiet state change.
- **Internal Padding:** None; content is centered via flexbox

### Navigation
- **Style:** Minimal footer bar with 1px top border in Border Zinc
- **Typography:** Brand name in Semibold 16px; links in Regular 14px
- **States:** Subtle background tint on hover (`hover:bg-muted/50`), color shift to foreground
- **Mobile:** Stacks vertically with gap spacing

## 6. Do's and Don'ts

### Do:
- **Do** use the dark mode as the default experience. The primary audience works in dim edit bays.
- **Do** keep body text at 16px (1rem) minimum. Respect the user's browser settings by using rem units throughout.
- **Do** cap line lengths at 65ch for comfortable reading.
- **Do** use weight contrast (400 vs 600 vs 700) to establish hierarchy, not just size changes.
- **Do** respect `prefers-reduced-motion` for all animations.
- **Do** use `font-variant-numeric: tabular-nums` for any data or version numbers.

### Don't:
- **Don't** use gradient text (`background-clip: text` with gradients). Decorative and never meaningful. Emphasis via weight or size only.
- **Don't** use side-stripe borders (colored left/right borders >1px on cards or alerts). Use full borders, background tints, or nothing.
- **Don't** wrap content in cards when plain text blocks suffice. Cards are the lazy answer.
- **Don't** use the hero-metric template (big number, small label, gradient accent). SaaS cliché.
- **Don't** create identical card grids (icon + heading + text, repeated endlessly).
- **Don't** use glassmorphism or blur effects as decoration.
- **Don't** use overly playful or consumer-friendly aesthetics that undermine the professional context of color grading work.
- **Don't** use crypto / neon-on-black aesthetic. Lutof is a production tool, not a speculative tech project.
- **Don't** use loud, oversaturated palettes that compete with the color-critical nature of the product's domain.
- **Don't** disable browser zoom (`user-scalable=no`). If the layout breaks at 200% zoom, fix the layout.
