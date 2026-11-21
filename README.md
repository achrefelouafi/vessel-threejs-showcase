# THE VESSEL — Procedural Three.js Architectural Showcase

Interactive **React 19 + TypeScript + Three.js (`0.187`)** procedural showcase of **The Vessel** (Hudson Yards, NYC), engineered with 1-to-1 mathematical and parameter parity to the companion Blender 5.1 Geometry Nodes graph (`The_Vessel_Procedural.blend`).

## Run Locally

```bash
npm install
npm run dev
```

Open `http://127.0.0.1:5173/` in your browser.

## Build for Production

```bash
npm run build
npm run preview
```

## Key Features
- **32+ Live Procedural Geometry Parameters** across 6 collapsible panels (`Silhouette & Scale`, `Honeycomb & Landings`, `Stairs & Structural Hull`, `Balustrades & Handrails`, `Base Plinth & Plaza`, `Materials & Atmosphere`).
- **6-Draw-Call Batched `Float32Array` Geometry Kernel** (`src/geometry/vesselGenerator.ts`) — rebuilds 116K–210K triangles in ~45–60 ms with zero memory leaks.
- **5 Architectural Presets**: `Hudson Classic`, `16-Story NYC`, `Twisted Crown`, `Ref Bowl`, and `Cathedral Keel`.
- **5 Smooth Fly-To Cameras** (`1`–`5`): `Hero`, `Oculus` (upward interior copper honeycomb view), `Detail`, `Iso`, and `Plaza`.
- **4 Calibrated Lighting Moods**: `Golden Hour`, `Dusk` (warm atrium uplighting), `Noon`, and `Studio` with HDR PMREM reflections and 4x MSAA post-processing.
- **5 Metallic Finishes**, **Wireframe Mode**, **Auto-Orbit (`Space`)**, **Clean Screenshot Mode (`H`)**, and **Live `.GLB` Export**.
