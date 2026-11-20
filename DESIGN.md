---
name: ARACNO Tactical Command
colors:
  surface: '#0f1419'
  surface-dim: '#0f1419'
  surface-bright: '#353a3f'
  surface-container-lowest: '#0a0f14'
  surface-container-low: '#171c21'
  surface-container: '#1b2025'
  surface-container-high: '#252a30'
  surface-container-highest: '#30353b'
  on-surface: '#dee3ea'
  on-surface-variant: '#bac9cc'
  inverse-surface: '#dee3ea'
  inverse-on-surface: '#2c3136'
  outline: '#849396'
  outline-variant: '#3b494c'
  surface-tint: '#00daf3'
  primary: '#c3f5ff'
  on-primary: '#00363d'
  primary-container: '#00e5ff'
  on-primary-container: '#00626e'
  inverse-primary: '#006875'
  secondary: '#7bd0ff'
  on-secondary: '#00354a'
  secondary-container: '#00a6e0'
  on-secondary-container: '#00374d'
  tertiary: '#a8ffd2'
  on-tertiary: '#003824'
  tertiary-container: '#5be9ad'
  on-tertiary-container: '#006645'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#9cf0ff'
  primary-fixed-dim: '#00daf3'
  on-primary-fixed: '#001f24'
  on-primary-fixed-variant: '#004f58'
  secondary-fixed: '#c4e7ff'
  secondary-fixed-dim: '#7bd0ff'
  on-secondary-fixed: '#001e2c'
  on-secondary-fixed-variant: '#004c69'
  tertiary-fixed: '#6ffbbe'
  tertiary-fixed-dim: '#4edea3'
  on-tertiary-fixed: '#002113'
  on-tertiary-fixed-variant: '#005236'
  background: '#0f1419'
  on-background: '#dee3ea'
  surface-variant: '#30353b'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  display-lg-mobile:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  headline-sm:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '600'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  telemetry-lg:
    fontFamily: JetBrains Mono
    fontSize: 20px
    fontWeight: '700'
    lineHeight: 24px
  telemetry-md:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 18px
  telemetry-sm:
    fontFamily: JetBrains Mono
    fontSize: 11px
    fontWeight: '400'
    lineHeight: 14px
  badge-code:
    fontFamily: JetBrains Mono
    fontSize: 10px
    fontWeight: '600'
    lineHeight: 12px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  gutter: 1rem
  gutter-sm: 0.5rem
  margin: 1.5rem
  margin-mobile: 0.75rem
  space-xs: 0.25rem
  space-sm: 0.5rem
  space-md: 1rem
  space-lg: 1.5rem
  space-xl: 2rem
---

## Brand & Style

This design system establishes a high-density, mission-critical tactical robotics interface built for real-time field operations, spatial orientation, and low-latency hardware control. The design tone combines military-grade telemetry precision with aerospace heads-up display (HUD) conventions. 

The aesthetic is futuristic yet functional: dark obsidian glass panels, high-contrast luminous vector accents, and crisp technical data readouts. It avoids purely decorative sci-fi tropes in favor of strict ergonomic legibility under high-stress, adverse lighting conditions. Operators must be able to parse joint actuator angles, kinematic velocity, thermal margins, and LiDAR obstacle matrices in a fraction of a second.

## Colors

The palette relies on absolute dark obsidian tones to optimize battery consumption on OLED field consoles and maximize ambient contrast for glowing tactical vectors.

- **Primary Accent (`#00E5FF` Neon Cyan):** Dedicated to primary action vectors, targeting crosshairs, selected actuator joints, and real-time command routing paths.
- **Secondary Accent (`#38BDF8` Electric Cyan):** Used for auxiliary readouts, telemetry graph curves, secondary borders, and interactive hover states.
- **Status Tiers:**
  - **Nominal / Online (`#10B981` Emerald):** Nominal gait synchronization, active servo lock, continuous telemetry link.
  - **Caution / Warning (`#F59E0B` Amber):** Over-torque alerts, joint friction, high-draw payload mode, sensor degradation.
  - **Critical / Emergency (`#EF4444` Crimson):** Kinematic failure, actuator stall, structural breach, emergency e-stop states.
- **Surfaces & Overlays:**
  - Background Base: `#0F1419`
  - Sub-panel Core: `#131B22`
  - Elevated Container: `#18222C`
  - Glass Container Fill: `rgba(15, 20, 25, 0.85)` with `rgba(0, 229, 255, 0.18)` 1px border.

## Typography

The typographic hierarchy is split intentionally between human-interface wayfinding and machine telemetry:

- **Inter** handles high-level navigational contexts, modal titles, operator instructions, and primary layout headings where proportional kerning maximizes reading speed.
- **JetBrains Mono** governs all quantitative and situational data: coordinate systems, Euler angles (Pitch/Roll/Yaw), battery wattage, serial protocol logs, LiDAR distances, and hardware error codes. Tabular figures ensure numerical alignment across real-time dynamic data columns without horizontal jitter.

## Layout & Spacing

The interface employs a responsive multi-panel tactical grid optimized for panoramic displays and ruggedized field tablets. 

- **Primary Command Cockpit (Desktop / Master Console):** 16-column fixed-ratio HUD with persistent peripheral telemetry sidebars (4 columns left, 8 columns center tactical viewport/LiDAR radar, 4 columns right joint actuator metrics).
- **Tablet Tactical Mode (Field Touch):** Reflows into an 8-column layout with collapsable diagnostics panels and persistent bottom-quarter virtual directional joysticks.
- **Mobile Handheld Mode:** Single-column stacked cards with swipeable instrument segments and a dominant status header.

Grid gutters remain strict at 16px to enforce high data density without visual collisions. Internal component padding enforces minimum 48px touch targets to accommodate gloved operation in tactical settings.

## Elevation & Depth

Visual hierarchy is communicated through translucent glassmorphic layering, subtle neon outer glows, and tactical border illumination rather than diffuse drop shadows.

- **Level 0 (Canvas Base):** Solid `#0F1419` deep field.
- **Level 1 (Docked Structural Panels):** Background `#131B22` with a 1px border in `rgba(0, 229, 255, 0.12)`.
- **Level 2 (HUD Floating Containers & Radar Scopes):** Frosted glass surface using `rgba(15, 20, 25, 0.85)` with `backdrop-filter: blur(12px)` and a 1px border in `rgba(0, 229, 255, 0.18)`.
- **Level 3 (Active Interacting Nodes & Modals):** Background `#18222C` with a 1px border in `rgba(0, 229, 255, 0.50)` and an ambient outer glow of `0 0 16px rgba(0, 229, 255, 0.25)`.
- **Critical Interventions (E-Stop / Alarms):** Hard-edged border highlight in `#EF4444` paired with an oscillating perimeter pulse (`0 0 20px rgba(239, 68, 68, 0.4)`).

## Shapes

The interface balances tactical industrial geometry with ergonomic touch radius. A base border-radius of 8px (`0.5rem`) is applied uniformly to modular panels, control pads, telemetry modules, and input zones. Interactive badges, posture toggles, and status pills utilize circular/pill curves to differentiate continuous controls from structural monitoring frames.

## Components

### Tactical Control Buttons
- Standard physical dimension: Minimum 48px height and width for gloved touch compatibility.
- Baseline: Surface `#18222C`, 1px border `rgba(0, 229, 255, 0.18)`, text uppercase `Inter` 12px semi-bold with `0.05em` letter-spacing.
- Active/Engaged State: Cyan neon fill `rgba(0, 229, 255, 0.15)`, solid border `#00E5FF`, accompanied by an outer aura glow `0 0 12px rgba(0, 229, 255, 0.35)`.
- Critical Emergency Stop (E-Stop): High-prominence red block (`#EF4444`) with high-contrast obsidian typography, haptic tactile response, and physical safety-lock border.

### Status Pills & Gait Indicators
- Height: 24px–28px, pill-shaped radius.
- Structure: 8px colored circular dot displaying active blink states next to monospace status strings (e.g., `TRIPOD GAIT: SYNCED`, `STANCE: CROUCH`).
- Border: `1px solid rgba(255, 255, 255, 0.08)`.

### Telemetry Cards
- Layout: Glassmorphic panel containing monospace numerical readouts, sparklines, and progress bars.
- Header: Sub-label in `JetBrains Mono` 11px muted gray-cyan (`#64748B`), data value in 20px bold neon cyan (`#00E5FF`).
- Border: Chamfered or 8px rounded corners with low-contrast cyan outlines.

### 2D LiDAR Radar Scope & Actuator HUD
- Scope container: Circular vector viewport rendered over a 50m concentric distance grid.
- Polar grid lines: `rgba(0, 229, 255, 0.15)` with cardinal direction markers (N, E, S, W) in monospace typography.
- Hexapod Leg Array: 6-point radial kinematic diagram displaying joint telemetry (Coxa, Femur, Tibia angles) with immediate dynamic color-shifts to Amber or Crimson under torque limit saturation.

### Virtual Vector Joystick
- Bounding Area: 120px circular touch-well with internal grid rings.
- Thumb Puck: 44px frosted circle with a center neon-cyan target indicator dot and directional vector guide showing velocity intensity.