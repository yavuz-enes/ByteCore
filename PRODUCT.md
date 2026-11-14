# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

React 19 + Vite + TypeScript with Tailwind CSS, Three.js / @react-three/fiber, Framer Motion, Zustand, Lucide Icons, and PeerJS (WebRTC)

## Users

Students, hackathon participants, STEM enthusiasts, and aspiring aerospace engineers participating in the NASA Space Apps Challenge (individual players or cooperative teams of up to 4 participants).

## Product Purpose

An interactive, educational space mission design game and flight simulation platform where players design, budget, configure, and launch space missions. Players discover real-world aerospace engineering trade-offs (mass, budget, power, communications, delta-v, and launch vehicle payload limits) and experience real-time launch telemetry and orbital mission evaluations.

## Positioning

Unlike disconnected orbital physics calculators or purely arcade rocket launchers, this platform integrates real NASA mission engineering constraints into a sleek aerospace mission control bridge. It uniquely combines 4-player WebRTC peer-to-peer cooperative multiplayer (Commander, Systems Engineer, Science Lead, Comms Officer), live synchronized telemetry, interactive 3D orbital mechanics visualization, and B1-level educational feedback.

## Operating Context

Modern desktop and tablet web browsers, classroom STEM workshops, remote hackathon team sessions, and solo self-paced learning environments.

## Capabilities and Constraints

- **Multiplayer Architecture**: Host creates a room with an easy 6-character room code; up to 3 teammates join via WebRTC (PeerJS) with zero server setup. Shared mission configuration, budget approvals, and synchronized launch countdown.
- **Solo Commander Mode**: Single-player option to seamlessly switch between all 4 console stations with built-in telemetry advisory feedback.
- **4 Crew Roles**:
  - *Mission Commander*: Selects mission target, orbital profile, launch vehicle, and triggers launch sequence.
  - *Systems Engineer*: Configures satellite bus, propulsion type, solar panels, and battery capacity.
  - *Science Lead*: Selects scientific payload instruments (cameras, spectrometers, radar, magnetometers) balancing mass, power, and science return.
  - *Communications Officer*: Selects high-gain/low-gain antennas, deep space ground station relays, and manages data downlink rates.
- **5 NASA Mission Scenarios**:
  - *Lunar Reconnaissance Orbiter*: Earth to Lunar polar orbit, mapping water ice.
  - *Mars Atmospheric & Sample Probe*: Earth-Mars Hohmann transfer, atmosphere entry and surface study.
  - *Europa Ocean Life Explorer*: Jupiter transfer, extreme radiation shielding and ice-penetrating radar.
  - *Asteroid Deflection & Resource Scout*: Deep space rendezvous, trajectory deflection test and mineral analysis.
  - *Free-form Sandbox Mission Architect*: Custom target celestial body, customizable budget and free trade-off experiments.
- **Interactive 3D Orbit Viewport**: Powered by Three.js and `@react-three/fiber`. Renders celestial bodies (Earth, Moon, Mars, Jupiter, Asteroid) with atmosphere glow, realistic orbital trajectory splines, and animated probe with deployable solar arrays and dish antenna.
- **Real-Time Launch Telemetry HUD**: Staged countdown, liftoff, Max-Q aerodynamic stress, stage separation, orbital insertion burn, solar panel deployment, and live science downlink data transmission.
- **Post-Flight Mission Report**: Detailed debriefing explaining why the mission succeeded or failed (Delta-V budget, power surplus/deficit, thermal and communication margins, science score, and team efficiency).
- **UI Copy Standard**: Simple, clear B1-level English. Concise, accessible, and free of unnecessary academic jargon.

## Brand Commitments

Faithfully adheres to the Minimalist Space Mission Command Deck design system defined in `DESIGN.md`:
- Strict 3-color palette: Primary `#1846FF` (Electric Royal Blue), Secondary `#B8B8FF` (Soft Lavender), Tertiary `#39FF14` (Neon Lime Green for all interactive controls).
- Deep dark void backgrounds: Canvas (`#060810`), Abyss (`#04050a`), Singularity (`#020306`).
- Prohibited colors: Zero reds, yellows, cyans, purples, or arbitrary grays.
- Decluttered top telemetry bar with dedicated Settings modal.
- Shape hierarchy: strictly `rounded-full` (9999px) for buttons, toggles, and pills; strictly `rounded-2xl` (16px) with 1px `#1846FF` borders for panels and cards.
- De-cluttered, high-density component cards stripped of explanatory fluff.

## Evidence on Hand

- `challange.html`: Official 2026 NASA Space Apps Challenge specification for "Space Mission Design Game".
- `DESIGN.md`: Comprehensive design token definitions, surface elevations, component patterns, and typography rules.
- `skills/`: Motion and UX performance guidelines.

## Product Principles

1. **Trade-offs Have Meaning**: Every payload instrument, solar cell, or antenna upgrade has tangible costs in mass, power, money, and launch requirements.
2. **Tactile Aerospace Command Bridge**: Mission control should feel high-tech, responsive, and grounded, with crisp metrics and immediate visual feedback.
3. **Cooperation Over Competition**: Team mode requires negotiation and shared responsibility to achieve mission success.
4. **Learning Through Doing**: Clear feedback explains the "why" behind mission results, empowering players to iterate, redesign, and triumph.

## Accessibility & Inclusion

- WCAG AA high-contrast ratios across all dark surfaces.
- Fully responsive layout for laptops, wide monitors, and tablets.
- Clear indicators, tactile state feedback, and readable monospace telemetry fonts.
