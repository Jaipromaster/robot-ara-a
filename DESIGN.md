---
name: ARACNO Tactical Command — Open World Edition
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
  outline: '#849396'
  outline-variant: '#3b494c'
  surface-tint: '#00daf3'
  primary: '#c3f5ff'
  primary-container: '#00e5ff'
  secondary: '#7bd0ff'
  tertiary: '#a8ffd2'
  error: '#ffb4ab'
  background: '#0f1419'
  on-background: '#dee3ea'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
  headline-md:
    fontFamily: Inter
    fontSize: 20px
    fontWeight: '600'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
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
---

## Brand & Style

This design system establishes a high-density, mission-critical tactical robotics interface built for real-time field operations, spatial orientation, and low-latency hardware control. The aesthetic combines dark obsidian glass panels, high-contrast luminous vector accents (`#00E5FF` Neon Cyan), and crisp technical telemetry readouts.

## Open-World 2D LiDAR Radar Architecture

The central Radar LiDAR 2D panel operates as a real-time interactive 24m × 24m open-world tactical map rendered on HTML5 Canvas:

- **Multi-Modal Locomotion:** Operators can drive ARACNO-6 freely via the 360° omnidirectional virtual joystick, keyboard (`WASD` / Arrow keys + `Q`/`E` yaw rotation), or autonomous click-to-navigate waypoints directly on the radar map.
- **Collision & Raycast Proximity Detection:** Circular beacons, structural walls, and perimeter boundaries enforce solid collision physics while a forward LiDAR sensor cone measures real-time obstacle distance in centimeters (`VÍA DESPEJADA` vs `OBSTÁCULO XX cm`).
- **Dynamic Camera & Telemetry:** Supports smooth spider-follow tracking, free-pan dragging, mouse-wheel zoom (`0.4x` to `2.7x`), fullscreen radar expansion, odometry tracking, and autonomous return-to-base (`A BASE`).
- **Synchronized Hexapod Kinematics:** The top-down 18-DOF vector chassis animates leg swing and stance phases dynamically according to live velocity, selected gait (`TRÍPODE`, `OLA`, `ONDULANTE`), and quick poses (`LEVANTARSE`, `SENTARSE`, `SALUDAR`, `BAILAR`).
