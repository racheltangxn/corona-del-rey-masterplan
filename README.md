# Corona del Rey Core Sample

A Vite + Three.js conceptual presentation of a sparse three-parcel Corona del Rey estate. The default view is a programming-model masterplan; selecting the Anchor Investor Estate opens the preserved high-detail Anchor Estate Core Sample.

## Live demo

[Open the deployed interactive masterplan](https://corona-core-sample.vercel.app/)

Source: [github.com/racheltangxn/corona-del-rey-masterplan](https://github.com/racheltangxn/corona-del-rey-masterplan)

The masterplan is conceptual only. Parcel geometry, routes, water features, access connections, and infrastructure are visual programming abstractions, not cadastral, topographic, engineering, environmental, or permitting data.

## Run

```bash
npm install
npm run build
npm run dev
```

Open the local URL Vite prints, usually `http://localhost:5173/`.

## Masterplan controls

- Full estate overview
- Focus Parcel 1 Operations and Service Core
- Focus Parcel 2 Primary Residential and Coastal Zone
- Focus Parcel 3 Residential, Water, and Future Value Zone
- Open the Anchor Estate Core Sample
- Toggle shared infrastructure
- Toggle future conversion markers

The overview includes eight sparse estate markers: one Anchor Investor Estate and seven simplified founding-family estates. It also shows conceptual roads, utility corridors, operations infrastructure, protected water features, agriculture, and a permit-dependent conceptual helipad marker. No private airstrip is modeled on the property.

## Core Sample controls

- Explore mode
- Focus estate
- Focus bunker
- Show bunker cutaway
- Reset camera
- Back to masterplan

The detailed Core Sample preserves the original hierarchy:

```text
CoreSample
├── StudioPlinth
├── TerrainCore
├── AnchorEstate
├── BunkerSubstructure
├── OceanSection
└── TemporaryPlaceholders
```

It is nested under `AnchorEstateCoreSample` within `CoreProject` and keeps the procedural volcanic terrain, rear arrival road, pool terrace, rocky cliff edge, animated ocean, vegetation, optional GLB loading, and unclipped bunker cutaway.

## Optional assets

Place future GLB files here:

```text
public/assets/terrain-core.glb
public/assets/anchor-estate.glb
public/assets/bunker-substructure.glb
```

The viewer remains fully runnable without them. Terrain and estate GLBs may receive the cutaway clipping plane. Bunker GLB materials remain unclipped, including material arrays, while bunker meshes continue to cast and receive shadows.
