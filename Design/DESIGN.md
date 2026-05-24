---
name: High-Performance Matrix
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#b9ccb2'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#84967e'
  outline-variant: '#3b4b37'
  surface-tint: '#00e639'
  primary: '#ebffe2'
  on-primary: '#003907'
  primary-container: '#00ff41'
  on-primary-container: '#007117'
  inverse-primary: '#006e16'
  secondary: '#b2ceb3'
  on-secondary: '#1e3623'
  secondary-container: '#364f3a'
  on-secondary-container: '#a4c0a5'
  tertiary: '#fff8f4'
  on-tertiary: '#442b10'
  tertiary-container: '#ffd5ae'
  on-tertiary-container: '#7a5b3c'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#72ff70'
  primary-fixed-dim: '#00e639'
  on-primary-fixed: '#002203'
  on-primary-fixed-variant: '#00530e'
  secondary-fixed: '#cdeace'
  secondary-fixed-dim: '#b2ceb3'
  on-secondary-fixed: '#08200f'
  on-secondary-fixed-variant: '#344c38'
  tertiary-fixed: '#ffdcbd'
  tertiary-fixed-dim: '#e7bf99'
  on-tertiary-fixed: '#2c1701'
  on-tertiary-fixed-variant: '#5d4124'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  headline-xl:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  title-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: '1.4'
    letterSpacing: '0'
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
    letterSpacing: '0'
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: '0'
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.08em
  mono-data:
    fontFamily: ui-monospace, monospace
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
    letterSpacing: '0'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
---

## Brand & Style
The design system is built on a "Terminal Modernism" aesthetic—a fusion of high-performance technical precision and contemporary minimalism. It targets developers, data scientists, and power users who value speed and clarity. 

The visual style is characterized by high-contrast functionalism. It utilizes a striking neon accent against deep, structured neutrals to evoke a sense of digital craftsmanship and "always-on" reliability. The emotional response should be one of clinical efficiency, cutting-edge innovation, and absolute focus.

## Colors
The palette is anchored by the "Matrix Green" primary color (#00FF41). This color is used sparingly as a high-intent signal for actions, progress, and success.

### Dark Mode (Primary)
In dark mode, surfaces utilize deep obsidian grays rather than pure black to maintain depth. Text levels scale from High-Emphasis Green or White down to muted grays for metadata.

### Light Mode
In light mode, the primary green is balanced with substantial white space and ink-black text to ensure WCAG 2.1 AAA compliance. The neon green is occasionally shifted to a slightly deeper forest-neon variant for small-text accessibility where necessary.

### Logic
- **Background:** Primary workspace color.
- **Surface:** Component backgrounds (cards, inputs).
- **On-Surface:** Text and icons residing on surfaces.
- **Accent:** Interactive triggers and critical status indicators.

## Typography
This design system utilizes **Inter** exclusively for its neutral, systematic character. The typographic scale is optimized for readability in data-heavy environments.

Headlines use tight tracking and bold weights to create a strong visual anchor. Body text prioritizes legibility with generous line heights. A secondary monospaced stack is reserved for technical data, code snippets, or ID strings to reinforce the technical brand narrative. All labels should be crisp and high-contrast.

## Layout & Spacing
The layout follows a rigorous **8px grid system**. Everything from component heights to inner padding must be a multiple of 8 (or 4 for micro-adjustments).

### Grid Model
- **Desktop:** 12-column fluid grid with 24px gutters. Max-width container of 1440px.
- **Tablet:** 8-column fluid grid with 16px gutters.
- **Mobile:** 4-column fluid grid with 16px gutters and 16px side margins.

Alignment should be "hard-edged"—elements should snap to the grid to maintain the "engineered" feel of the interface. Use generous vertical rhythm (xl spacing) between major sections to prevent visual clutter.

## Elevation & Depth
Depth is achieved through **Tonal Layering** rather than traditional soft shadows.

In Dark Mode, the z-axis is represented by increasing the lightness of the gray surface. The background is the darkest, while modals and dropdowns are the lightest grays. 

For interactive states, use **Inner Glows** or **Low-contrast Outlines** in the primary green to indicate focus. Shadows, when used for high-level overlays (modals), should be sharp and high-density, appearing more like a "drop-off" than a soft blur. Semi-transparent dark backdrops (70% opacity) are used to dim the background when modals are active.

## Shapes
The shape language is "Soft-Tech." All standard UI components (inputs, buttons, cards) utilize an **8px (0.5rem)** corner radius. 

This specific radius bridges the gap between the aggressive sharpness of a 0px terminal and the overly consumer-friendly 16px+ radius. Larger containers, like main content areas or hero sections, may use 1rem (16px) for distinct containment, while small utility tags and chips should remain at 4px or 8px. Never use full pill-shapes; maintain the structured rectangular integrity.

## Components

### Buttons
- **Primary:** Solid #00FF41 background with #001405 text. No border.
- **Secondary:** Ghost style. Transparent background, 1px border of #00FF41, text in #00FF41.
- **Tertiary:** Text-only with an underline or icon.

### Input Fields
Inputs use a dark-tinted surface with a subtle 1px border. Upon focus, the border transitions to Primary Green with a subtle 2px outer glow (0% blur) to simulate a terminal cursor's intensity.

### Cards
Cards are flat with a 1px border (color: Surface-Stroke). There is no drop shadow; instead, use a slight background color shift on hover to indicate interactivity.

### Chips & Badges
Small, rectangular containers with 4px border radius. Use subtle Primary Green backgrounds with 10-15% opacity for "active" states, keeping the text sharp and legible.

### Lists
Lists should use thin dividers (1px) with high horizontal padding. Hover states on list items should utilize a "scan-line" effect or a subtle left-hand accent bar in Primary Green.