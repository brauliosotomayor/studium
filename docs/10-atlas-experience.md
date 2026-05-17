# Map UX & Discovery Logic

**Version:** Phase II · 2026-05-17  
**Status:** Experience specification (static concept on site; app not built)

---

## Design intent

The Studium map is a **living atlas**, not a booking grid.

| Feel | Avoid |
|------|-------|
| Sacred, cinematic, intentional | Crowded pin spam |
| Slow zoom; breathing layout | Yelp density |
| Constellation corridors | Airbnb price cards |
| Stewardship gravity | Influencer discovery |

**Reference aesthetics:** Antique atlases, Japanese craft monographs, museum catalogs, field journals—earth tones, parchment, minimal type (see `docs/index.html`).

---

## Map layers

| Layer | Default | Description |
|-------|---------|-------------|
| **Base** | On | Parchment/ocean minimal cartography; low political noise |
| **Corridors** | On | Curved routes connecting node clusters—not straight geodesics |
| **Nodes** | On | Illuminated (active) vs dim (candidate) |
| **Archetypes** | Off | Color overlay per `06-knowledge-archetypes.md` |
| **Stewardship** | Off | High-sensitivity halo; indigenous/ecological boundaries |
| **Constellation phase** | Metadata | 3 / 5 / 13 / 50 / 200 ring indicator at zoom out |

---

## Zoom levels

| Level | View | Behavior |
|-------|------|----------|
| **0 — Planet** | Global | 13 constellation clusters as soft regions; no pin labels |
| **1 — Corridor** | Continental | Corridor name + route arc; node count badge |
| **2 — Region** | Country/subregion | Nodes visible; craft labels on hover |
| **3 — Place** | Local | Master/steward card; application CTA (future) |
| **4 — Workshop** | Site (future) | Interior documentation; archive media |

**Rule:** Never show Level 3+ for High sensitivity without application acceptance.

---

## Corridor visualization

```
     ●───────●  Murano
    ╱         ╲
   ● Florence ●──── Carrara
    ╲         ╱
     ●───────●  Cremona

  Italian Master Craft Corridor (arc, not box)
```

- Corridors drawn as **great-circle-inspired curves** following cultural routes.  
- Sub-clusters (Tuscany, Veneto) appear only at Level 2+.  
- Click corridor → filter rail locks to corridor + shows registry excerpt.

---

## Filtering

| Filter | Type | Notes |
|--------|------|-------|
| Corridor | Single or multi | Primary navigation |
| Knowledge Archetype | Multi | OR within, AND with corridor |
| Steward Type | Craft Master / Land Steward | |
| Sensitivity | Show/hide High | Default: hide High until “serious seeker” toggle |
| Founder Phase | Seed / 13 / 50 | Educational overlay |
| Duration | Visit / Apprenticeship / Residency | From experience catalog (future) |
| Indigenous / Ecological | Y/N | Steward-gated visibility |

**No filters for:** price, rating, popularity, “near me” tourism.

---

## Constellation behavior

| Phase | Visual |
|-------|--------|
| **3 (Seed)** | Three bright stars; rest constellation outline only |
| **5** | First ring complete; pulse animation on new acceptance |
| **13** | Full founding constellation; 13 cluster labels |
| **50** | Density increase; dim nodes activate |
| **200** | Global mesh; archive search primary |

Animation: **slow breathe** (4–6s cycle)—never gamified sparkle.

---

## Node card (discovery)

```
┌─────────────────────────────────┐
│ [archetype badge]  Medium sens. │
│ Vineyard Stewardship            │
│ Douro Valley · Portugal         │
│ Iberian Craft & Land Corridor   │
│ ─────────────────────────────── │
│ Terraced viticulture…           │
│ [Apply to learn]  not [Book now]│
└─────────────────────────────────┘
```

---

## Sensitivity layers

| Overlay | Visual | Interaction |
|---------|--------|-------------|
| **Indigenous** | Soft amber boundary | Click → stewardship code summary |
| **Ecological** | Green contour | Seasonal availability hint |
| **High sensitivity** | Node hidden until intent declared | Extra application fields |

---

## Static site (Phase II)

`docs/index.html` implements:

- Hero + manifesto  
- Triangle section  
- **Corridor cards** (top corridors by node count)  
- **Founding 13** summary  
- **Archetype grid**  
- **Map concept** panel with brand imagery from `docs/assets/`  

Full interactive map = Phase III (after IA + stack).

---

## Accessibility & performance

- Map alternative: **accessible list view** with same filters  
- Low-motion mode disables breathe animation  
- No autoplay video on map  
- Image lazy-load; corridor data from CSV fetch (future)

---

## Related artifacts

- `05-corridor-registry.md`  
- `06-knowledge-archetypes.md`  
- `07-founding-13.md`  
- `08-stewardship-framework.md`  
- `data/studium_atlas_master.csv`
