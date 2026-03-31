# Regen Atlas

**[Live](https://ra-april-26.vercel.app)** · **[Production](https://regenatlas.xyz)**

Open-source registry of tokenized environmental assets, ecological actions, and regenerative actors — mapped to 185 bioregions.

## Stack

- **Frontend:** React + TypeScript + Vite + Tailwind CSS
- **Map:** Mapbox GL JS (react-map-gl) with GeoJSON bioregion boundaries, composite cluster layers, spiderfy
- **Data:** Supabase (PostgreSQL) — 505 assets, 224 actions, 27 actors across 6 protocols
- **Images:** 247 AI-generated bioregion landscapes (FLUX 1.1 Pro via Replicate)

## Features

- **Bioregion Explorer** — 185 One Earth bioregions with asset/action/actor counts, PFP images, tabbed detail panels
- **Entity Filtering** — Assets (Type/Issuer/Chain), Actions (Protocol/SDG/Time), Actors (Orgs/Agents)
- **Action Grouping** — Actions at same location with same base title bundled in panel, deduped on map at high zoom
- **Actor Views** — Organizations and AI agents (owockibot) with collapsible accordion + detail cards
- **List Project** — Formspree-powered submission form for assets, actors, and actions
- **Mobile Responsive** — Entity toggle pills, full filter modal with Protocol/SDG support, 44px touch targets

## Development

```bash
npm install
npm run dev        # localhost:5173
npm run build      # production build to dist/
```

Requires `.env` with:
```
VITE_SUPABASE_URL=...
VITE_SUPABASE_ANON_KEY=...
VITE_MAPBOX_ACCESS_TOKEN=...
```

## Protocols Tracked

Toucan, Regen Network, Hedera Guardian, Atlantis, Ecocerts (Gainforest), Silvi, Glow

## License

MIT
