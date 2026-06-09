---
name: Signal Intelligence System
colors:
  surface: '#f7f9fb'
  surface-dim: '#d8dadc'
  surface-bright: '#f7f9fb'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f2f4f6'
  surface-container: '#eceef0'
  surface-container-high: '#e6e8ea'
  surface-container-highest: '#e0e3e5'
  on-surface: '#191c1e'
  on-surface-variant: '#444651'
  inverse-surface: '#2d3133'
  inverse-on-surface: '#eff1f3'
  outline: '#757682'
  outline-variant: '#c5c5d3'
  surface-tint: '#4059aa'
  primary: '#00236f'
  on-primary: '#ffffff'
  primary-container: '#1e3a8a'
  on-primary-container: '#90a8ff'
  inverse-primary: '#b6c4ff'
  secondary: '#00687a'
  on-secondary: '#ffffff'
  secondary-container: '#57dffe'
  on-secondary-container: '#006172'
  tertiary: '#00311f'
  on-tertiary: '#ffffff'
  tertiary-container: '#004a31'
  on-tertiary-container: '#27c38a'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dce1ff'
  primary-fixed-dim: '#b6c4ff'
  on-primary-fixed: '#00164e'
  on-primary-fixed-variant: '#264191'
  secondary-fixed: '#acedff'
  secondary-fixed-dim: '#4cd7f6'
  on-secondary-fixed: '#001f26'
  on-secondary-fixed-variant: '#004e5c'
  tertiary-fixed: '#6ffbbe'
  tertiary-fixed-dim: '#4edea3'
  on-tertiary-fixed: '#002113'
  on-tertiary-fixed-variant: '#005236'
  background: '#f7f9fb'
  on-background: '#191c1e'
  surface-variant: '#e0e3e5'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  headline-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  title-md:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-sm:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  technical-data:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: -0.01em
  label-caps:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
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
  grid_columns_mobile: '4'
  grid_columns_desktop: '12'
  gutter: 16px
---

## Brand & Style
The design system is engineered for a mobile-first network monitoring platform that bridges the gap between field engineering and executive-level analytics. The brand personality is **Professional, Reliable, and Data-Driven**, prioritizing clarity over decoration. 

The aesthetic follows a **Modern Corporate** direction, heavily influenced by Material Design 3. It utilizes a structured "Container-on-Surface" architecture to manage high information density without overwhelming the user. The style emphasizes:
- **Geographic Intelligence:** Seamless integration of map layers with floating UI controls.
- **Visual Precision:** Using a rigorous grid to align technical metrics and signal data.
- **Operational Clarity:** High-contrast status indicators that provide immediate "at-a-glance" understanding of network health.

## Colors
The palette is rooted in **Deep Blue (#1E3A8A)** to establish institutional trust. **Cyan (#06B6D4)** serves as the "Connectivity" color, used for active data streams, signal waves, and primary actions.

- **Primary (Deep Blue):** Use for top-level navigation, primary buttons, and branding elements.
- **Secondary (Cyan):** Use for interactive technical elements, toggles, and data points related to live connectivity.
- **Success (Emerald):** Reserved strictly for "Good" signal strength, successful syncs, and active cell towers.
- **Neutral/Surface:** The system uses a multi-tier grayscale. `F8FAFC` is the base background, while pure `FFFFFF` is used for elevated cards to create subtle contrast.
- **Dark Mode:** In dark mode, the primary surface shifts to `111827`, with components using a slightly lighter `1F2937` to maintain depth.

## Typography
The typography system uses **Inter** for its exceptional legibility in data-heavy environments. To distinguish between human-readable UI and raw machine data, **JetBrains Mono** is introduced for technical metrics.

- **Headlines:** Use Bold weights for section titles to anchor the layout.
- **Body:** Regular weight for general descriptions; Medium weight for emphasis within cards.
- **Technical Metrics:** Values such as RSRP, RSRQ, and Frequencies must always be set in `technical-data` (JetBrains Mono) to ensure tabular numbers align perfectly for visual comparison.
- **Labels:** Use `label-caps` for small metadata descriptors or table headers to provide a clear structural hierarchy.

## Layout & Spacing
The system utilizes an **8px linear scale** for consistent rhythmic spacing. 

- **Mobile Layout:** 4-column fluid grid with 16px side margins. Cards usually span the full width or 2 columns for smaller metric tiles.
- **Web Dashboard:** 12-column fixed grid (max-width 1440px) or fluid (for map views). Use a "Master-Detail" pattern where a side panel (4 columns) displays metric specifics while the map (8 columns) provides spatial context.
- **Density:** In mobile monitoring views, use `sm` (8px) padding for cards to maximize data visibility. In administrative settings, use `md` (16px) for better readability.

## Elevation & Depth
Depth is used to represent the importance and interactivity of data layers. Following Material 3 principles:

- **Level 0 (Surface):** The background (`F8FAFC`). No shadow.
- **Level 1 (Card):** Used for data modules. Subtle 1px border (`E2E8F0`) and a very soft ambient shadow: `0 1px 3px rgba(0,0,0,0.05)`.
- **Level 2 (Floating Controls):** Map zoom buttons, filter chips, and FABs. Medium shadow: `0 4px 6px rgba(0,0,0,0.1)`.
- **Level 3 (Modals/Overlays):** Darkened backdrops with high-diffused shadows to focus user attention on critical alerts or signal test results.

## Shapes
The shape language is "Approachable Geometric." A consistent **8px (0.5rem)** radius is applied to standard UI elements like cards, input fields, and buttons.

- **Containers:** 8px radius (`rounded-md`).
- **Large Sections/Sheets:** 16px radius (`rounded-lg`) on top corners for mobile bottom sheets.
- **Status Badges:** Fully rounded (pill-shaped) to distinguish them from interactive buttons.
- **Iconography:** Use rounded-corner icons to match the UI's softness. Avoid sharp 90-degree angles in custom signal strength illustrations.

## Components
- **Signal Strength Gauges:** Use a 5-bar vertical histogram. Color bars based on status: Emerald (Excellent), Cyan (Good), Amber (Fair), Rose (Poor/No Signal).
- **Connectivity Badges:** Small pill-shaped tags (e.g., "5G", "LTE", "Roaming") using a Secondary (Cyan) background at 10% opacity with a solid Cyan border.
- **Analytics Cards:** White background, 8px radius, containing a title-md header, a JetBrains Mono primary metric, and a small sparkline chart at the bottom.
- **Map Controls:** Floating vertical stacks of square buttons (40x40px) with 8px radius, positioned on the right side of the viewport.
- **Sync Status Banner:** A full-width bar appearing below the header. Use `Amber` for "Offline - Sync Pending" and `Emerald` for "All Data Synced."
- **Buttons:**
    - *Primary:* Solid Deep Blue with white text.
    - *Secondary:* Outline Cyan with 1px border.
    - *Actionable Metric:* A card that acts as a button, providing a subtle hover state shift from Level 1 to Level 2 elevation.