---
name: Slate & Silver Smart Dashboard
colors:
  surface: '#0b1326'
  surface-dim: '#0b1326'
  surface-bright: '#31394d'
  surface-container-lowest: '#060e20'
  surface-container-low: '#131b2e'
  surface-container: '#171f33'
  surface-container-high: '#222a3d'
  surface-container-highest: '#2d3449'
  on-surface: '#dae2fd'
  on-surface-variant: '#c5c6cb'
  inverse-surface: '#dae2fd'
  inverse-on-surface: '#283044'
  outline: '#8e9195'
  outline-variant: '#44474a'
  surface-tint: '#c1c7cf'
  primary: '#ffffff'
  on-primary: '#2b3137'
  primary-container: '#dde3eb'
  on-primary-container: '#5f656c'
  inverse-primary: '#595f66'
  secondary: '#b9c8de'
  on-secondary: '#233143'
  secondary-container: '#39485a'
  on-secondary-container: '#a7b6cc'
  tertiary: '#ffffff'
  on-tertiary: '#28313b'
  tertiary-container: '#dae3f0'
  on-tertiary-container: '#5c6570'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#dde3eb'
  primary-fixed-dim: '#c1c7cf'
  on-primary-fixed: '#161c22'
  on-primary-fixed-variant: '#41474e'
  secondary-fixed: '#d4e4fa'
  secondary-fixed-dim: '#b9c8de'
  on-secondary-fixed: '#0d1c2d'
  on-secondary-fixed-variant: '#39485a'
  tertiary-fixed: '#dae3f0'
  tertiary-fixed-dim: '#bdc8d3'
  on-tertiary-fixed: '#131d25'
  on-tertiary-fixed-variant: '#3e4852'
  background: '#0b1326'
  on-background: '#dae2fd'
  surface-variant: '#2d3449'
  slate-900: '#0F172A'
  slate-800: '#1E293B'
  charcoal-black: '#020617'
  silver-accent: '#E5E7EB'
  glass-border: rgba(255, 255, 255, 0.1)
typography:
  headline-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Plus Jakarta Sans
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-md:
    fontFamily: Plus Jakarta Sans
    fontSize: 20px
    fontWeight: '500'
    lineHeight: 28px
  body-lg:
    fontFamily: Plus Jakarta Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Plus Jakarta Sans
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  label-caps:
    fontFamily: Plus Jakarta Sans
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.1em
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 18px
    fontWeight: '500'
    lineHeight: 24px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  container-max: 480px
  gutter: 1.5rem
  margin-x: 1rem
  stack-sm: 0.5rem
  stack-md: 1rem
  stack-lg: 2rem
---

## Brand & Style

The design system embodies **High-End Minimalist Tech**, specifically tailored for a luxury smart home environment. It moves away from generic colorful interfaces toward a sophisticated, monochromatic palette that feels architectural and permanent.

The aesthetic combines elements of **Minimalism** and **Glassmorphism**. It utilizes generous whitespace (negative space) to reduce cognitive load and create a sense of calm. Instead of physical neomorphism, it employs refined depth through semi-transparent layers, backdrop blurs, and high-precision borders that mimic machined aluminum and polished glass.

The UI should evoke a sense of \"Invisible Technology\"—powerful, silent, and effortlessly premium. It is designed for a target audience that values discretion, material quality, and modern aesthetics.

## Colors

The system uses a strictly monochromatic, dark-mode-first palette. The primary color is a bright off-white used for high-contrast text and critical icons, while the neutral foundation is built on deep charcoals and slate grays.

- **Primary:** An off-white/silver (`#E2E8F0`) for maximum legibility against dark backgrounds.
- **Secondary:** A muted slate (`#94A3B8`) for secondary information and inactive states.
- **Metallic Silver:** Used sparingly as an accent for highlights, thin borders, and active indicators to provide a \"machined\" feel.
- **Backgrounds:** The interface utilizes `charcoal-black` for the main canvas and `slate-900/800` for container layers to create depth without relying on pure black.

No vibrant colors (specifically yellow) are to be used, maintaining a rigorous luxury atmosphere.

## Typography

**Plus Jakarta Sans** provides a clean, contemporary feel with geometric clarity, serving as the primary typeface for all UI elements. To emphasize the technical nature of a smart home system, **JetBrains Mono** is introduced specifically for numeric data and sensor readings (temperature, humidity, lux levels).

Headlines use tighter letter spacing and semi-bold weights to appear \"locked-in\" and authoritative. Labels for metadata or categories should be set in all caps with increased letter spacing for a premium, architectural look. 

For mobile, headlines scale down to prevent text wrapping on smaller control cards, ensuring the dashboard remains usable on hand-held devices.

## Layout & Spacing

The layout is a **Fixed Grid** centered within a `480px` maximum width to optimize for mobile-first smart home control. On desktop, the dashboard remains a centered column to maintain its focused, \"app-like\" feel.

A rhythmic 8px base unit (0.5rem) governs all spacing. 
- **Margins:** A standard 24px (1.5rem) gutter exists between major layout sections.
- **Internal Padding:** Cards use 20px or 24px internal padding to ensure content feels airy and un-cramped.
- **Reflow:** On tablets, the layout may expand to a 2-column grid of cards, but the dashboard always maintains its structured, symmetrical appearance.

## Elevation & Depth

Hierarchy is achieved through **Tonal Layers** and **Glassmorphism** rather than traditional drop shadows.

- **Base Layer:** The canvas uses the darkest charcoal.
- **Mid Layer (Cards):** Containers use a slightly lighter slate with a very subtle `backdrop-filter: blur(16px)` and a semi-transparent background (`rgba(30, 41, 59, 0.7)`).
- **Edges:** Depth is defined by **Low-contrast outlines**. Every card has a 1px solid border using the `glass-border` variable, creating a sharp, \"etched\" look.
- **Shadows:** When used, shadows are ambient and diffused—never dark or heavy. Use a large blur (20px+) with low opacity (15%) tinted with the slate color to simulate a soft glow rather than a harsh drop.

## Shapes

The shape language is **Rounded** (0.5rem base), providing a balance between technical precision and modern comfort. 

- **Small elements (Chips, small buttons):** 0.5rem.
- **Standard Cards:** 1rem (`rounded-lg`).
- **Interactive Toggles:** 1.5rem (`rounded-xl`) or full pill-shape for sliders.

This softening of the corners prevents the monochromatic and dark theme from feeling too aggressive or \"brutalist,\" ensuring it remains inviting for home use.

## Components

### Buttons
Primary buttons use a \"metallic\" treatment—subtle gradients from slate-200 to slate-400 with dark text. Secondary buttons are ghost-style with the 1px `glass-border`. Active states are indicated by a soft silver glow.

### Cards
Cards are the primary container. They must feature a subtle glass effect and the signature 1px border. They should never have a heavy shadow.

### Sensor Monitors
Use **JetBrains Mono** for the numeric values. Pair the number with a thin, high-quality icon. Use \"Slate-400\" for units (e.g., °C, %) to keep them secondary to the value.

### Toggles & Controls
Switches should be oversized for ease of touch. The \"On\" state should use the `silver-accent` to clearly differentiate from the \"Off\" (slate-800) state. 

### Communication Terminal
The communication log should be treated as a sunken element using a darker background than the base canvas to simulate a terminal screen recessed into a physical panel.

### Iconography
Use thin-stroke (Light or Thin weight) line icons. Icons should be strictly monochromatic—silver for active/important and slate-500 for decorative.
