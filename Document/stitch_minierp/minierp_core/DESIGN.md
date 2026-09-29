---
name: MiniERP Core
colors:
  surface: '#f7f9ff'
  surface-dim: '#d7dadf'
  surface-bright: '#f7f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f1f4f9'
  surface-container: '#ebeef3'
  surface-container-high: '#e5e8ee'
  surface-container-highest: '#e0e3e8'
  on-surface: '#181c20'
  on-surface-variant: '#424754'
  inverse-surface: '#2d3135'
  inverse-on-surface: '#eef1f6'
  outline: '#727785'
  outline-variant: '#c2c6d6'
  surface-tint: '#005ac2'
  primary: '#0058be'
  on-primary: '#ffffff'
  primary-container: '#2170e4'
  on-primary-container: '#fefcff'
  inverse-primary: '#adc6ff'
  secondary: '#505f76'
  on-secondary: '#ffffff'
  secondary-container: '#d0e1fb'
  on-secondary-container: '#54647a'
  tertiary: '#924700'
  on-tertiary: '#ffffff'
  tertiary-container: '#b75b00'
  on-tertiary-container: '#fffbff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#adc6ff'
  on-primary-fixed: '#001a42'
  on-primary-fixed-variant: '#004395'
  secondary-fixed: '#d3e4fe'
  secondary-fixed-dim: '#b7c8e1'
  on-secondary-fixed: '#0b1c30'
  on-secondary-fixed-variant: '#38485d'
  tertiary-fixed: '#ffdcc6'
  tertiary-fixed-dim: '#ffb786'
  on-tertiary-fixed: '#311400'
  on-tertiary-fixed-variant: '#723600'
  background: '#f7f9ff'
  on-background: '#181c20'
  surface-variant: '#e0e3e8'
typography:
  display:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  headline-sm:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: '1.4'
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: '1.5'
  label-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '600'
    lineHeight: '1'
    letterSpacing: 0.01em
  data-tabular:
    fontFamily: Inter
    fontSize: 13px
    fontWeight: '400'
    lineHeight: '1.4'
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 32px
  gutter: 16px
  margin-mobile: 16px
  margin-desktop: 32px
---

## Brand & Style
The design system is anchored in a **Modern Minimalist** aesthetic specifically tailored for personal and domestic resource management. It prioritizes cognitive ease and productivity, transforming complex ERP data into a calm, navigable environment. 

The style draws inspiration from industrial-grade ERPs like ERPNext but softens the edges for a domestic context. It utilizes expansive whitespace, a disciplined neutral palette, and a clear functional hierarchy. The emotional response should be one of "controlled order"—the user should feel that their finances, inventory, and tasks are structured and manageable. There is a heavy focus on clarity over decoration, using subtle borders and intentional typography to define regions rather than heavy fills or aggressive shadows.

## Colors
The color strategy employs a high-ratio of "Ink on Paper" neutrals to ensure longevity and reduce interface fatigue.

- **Primary:** A professional, mid-tone blue (#3B82F6) used for primary actions, active states, and focus indicators.
- **Neutrals:** The foundation is built on `#F8F9FA` for page backgrounds and pure `#FFFFFF` for cards and surface elements. Text utilizes `#212529` to maintain high legibility without the harshness of pure black.
- **Semantic Palette:** Success, Error, and Warning states use slightly desaturated versions of their respective hues to remain visible but not jarring within the minimalist framework.
- **Borders:** `#E9ECEF` serves as the primary structural divider, creating subtle definition between sections.

## Typography
This design system utilizes **Inter** for its systematic, utilitarian nature and excellent legibility at small sizes.

- **Hierarchy:** Use `Display` and `Headline-md` sparingly for dashboard overviews. 
- **Data Density:** `body-md` is the workhorse for general interface text. For data-heavy tables, use `data-tabular` (13px) with tabular lining figures enabled to ensure numeric columns align perfectly.
- **Labels:** Labels for inputs and metadata use `label-sm` in a medium or semi-bold weight to distinguish them clearly from the user data they describe.

## Layout & Spacing
The layout follows a **Fluid Grid** model with a max-width container of 1440px for desktop to prevent line lengths from becoming unreadable.

- **Grid:** A 12-column grid system is used for desktop, collapsing to 4 columns for mobile.
- **Rhythm:** An 8px linear scale (4px for micro-adjustments) governs all margins and paddings. 
- **Density:** Use `md` (16px) for standard component padding and `lg` (24px) for page-level sectioning. Tables should utilize a "Compact" vertical rhythm (8px row padding) to maximize information density without sacrificing touch targets or legibility.
- **Sidenav:** A fixed 240px sidebar is standard for desktop navigation, collapsing to an icon-only rail or drawer on smaller viewports.

## Elevation & Depth
Elevation is handled with extreme restraint to maintain the minimalist philosophy.

- **Flat Foundation:** Most surfaces exist on the same Z-plane, separated by `1px` borders in `#E9ECEF`.
- **Minimal Shadows:** When depth is required (e.g., a raised Card or a Dropdown), use a single, highly diffused shadow: `0 4px 12px rgba(0, 0, 0, 0.05)`. 
- **Tonal Layers:** Use background color shifts (`#F8F9FA` vs `#FFFFFF`) to indicate nesting or hierarchy rather than shadows.
- **Active States:** Active buttons or focused inputs should not "pop" with shadow; instead, use a `2px` solid primary color border or a subtle tonal shift.

## Shapes
The shape language is "Soft-Modern." UI elements follow a `8px` (standard) to `12px` (large) corner radius.

- **Standard Components:** Buttons, Input fields, and Chips use `rounded-md` (8px).
- **Containers:** Mat-cards and large surface areas use `rounded-lg` (12px) to provide a friendlier, domestic feel.
- **Status Indicators:** Small tags and badges may use a full pill-shape (999px) to distinguish them from interactive buttons.

## Components
- **Buttons:** Use `Mat-flat-button` as the primary style. Avoid heavy gradients. Height should be 36px for standard and 44px for main actions.
- **Cards (Mat-card):** Use a 1px solid border (`#E9ECEF`) instead of a shadow by default. Only add the minimal shadow on hover if the card is interactive.
- **Tables (Mat-table):** Horizontal dividers only. Remove vertical grid lines to increase "air." Headers should be `label-sm` in all-caps or semi-bold with a subtle grey background.
- **Inputs:** Outlined style with an 8px radius. Label should be persistent or use the floating label pattern provided by Angular Material.
- **Chips:** Small, low-contrast background with `primary` or `semantic` text colors. No borders on chips unless they are de-selectable.
- **Sidenav:** Use a clean, vertical list with icon + text. Active states should be indicated by a vertical 4px bar on the left edge and a subtle blue tint on the background.
- **Summary Tiles:** Specialized small cards for the dashboard containing a "Label," "Value," and "Trend Indicator" (Sparkline or percentage) to provide an immediate snapshot of ERP status.