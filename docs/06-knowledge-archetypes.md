# Knowledge Archetype System

**Version:** Phase II · 2026-05-17  
**Status:** Canonical taxonomy for atlas nodes, filters, and stewardship rules

---

## Purpose

Knowledge Archetypes classify **what kind of transmission** occurs at a node—not merely what industry it resembles. Archetypes drive map overlays, application questions, steward review paths, and archive structure.

**Nine canonical archetypes.** No node is archetype-only; craft and place always remain primary.

---

## Canonical archetypes

### 1. Textile & Fiber Craft

| Field | Definition |
|-------|------------|
| **Inclusion** | Weaving, dyeing, embroidery, quilting, basketry, felt, loom traditions |
| **Exclusion** | Industrial fashion production; machine-only textile tours |
| **Overlap** | Material Craft (when fiber is structural); Music & Storytelling (narrative quilts) |
| **Examples** | Kente weaving (Ghana), Zapotec weaving (Oaxaca), Murano-adjacent Florentine textiles, Gee's Bend quilting |
| **UX** | Loom/workshop imagery; duration filters for multi-week dye apprenticeships |
| **Extensibility** | Sub-tags: `natural_dye`, `ceremonial_cloth`, `backstrap` |

### 2. Material Craft

| Field | Definition |
|-------|------------|
| **Inclusion** | Metal, glass, wood, stone, lacquer, bronze, ceramics, sculpture |
| **Exclusion** | Mass manufacturing; replica souvenir production |
| **Overlap** | Architecture & Building Craft (structural stone); Instrument & Music Craft |
| **Examples** | Murano glass, lost-wax bronze (Burkina Faso), sword forging (Japan), Shona sculpture |
| **UX** | Material close-ups; heat/forging safety disclosures in application |
| **Extensibility** | Sub-tags: `forging`, `casting`, `carving`, `glass` |

### 3. Architecture & Building Craft

| Field | Definition |
|-------|------------|
| **Inclusion** | Masonry, adobe, joinery, plaster, tile, dry stone, temple carpentry |
| **Exclusion** | Commercial construction contracting without transmission intent |
| **Overlap** | Land Stewardship (land-forming walls, terraces); Material Craft |
| **Examples** | Dry stone walling (Portugal), zellige (Morocco), adobe (New Mexico), temple carpentry (Nara) |
| **UX** | Site-based experiences; longer residency defaults |
| **Extensibility** | Sub-tags: `sacred_building`, `vernacular`, `earthen` |

### 4. Land Stewardship

| Field | Definition |
|-------|------------|
| **Inclusion** | Regenerative agriculture, forestry, pastoral systems, ethnobotany, fire ecology, water harvesting |
| **Exclusion** | Greenwashing retreats; property speculation framed as ecology |
| **Overlap** | Food & Fermentation (when harvest is the practice); Navigation (place literacy) |
| **Examples** | Douro vineyard stewardship, chinampa agriculture, cultural burning (California), satoyama (Japan) |
| **UX** | Seasonal availability; ecological prerequisite fields in applications |
| **Extensibility** | Sub-tags: `indigenous_stewardship`, `vineyard`, `forest`, `arid_land` |

### 5. Food & Fermentation

| Field | Definition |
|-------|------------|
| **Inclusion** | Fermentation, wine in qvevri, bread culture, coffee processing, preservation |
| **Exclusion** | Restaurant tourism; cooking classes without lineage |
| **Overlap** | Land Stewardship (agroforestry coffee); Material Craft (vessel-making) |
| **Examples** | Qvevri winemaking (Georgia), coffee fermentation (Colombia), harvest traditions |
| **UX** | Harvest calendar overlay; alcohol/regulatory flags |
| **Extensibility** | Sub-tags: `wine`, `ferment`, `coffee`, `ceremonial_food` |

### 6. Maritime & Watercraft

| Field | Definition |
|-------|------------|
| **Inclusion** | Boat building, skin-sewn kayaks, reed watercraft, maritime survival craft |
| **Exclusion** | Recreational boating; cruise tourism |
| **Overlap** | Navigation & Wayfinding; Material Craft (wood joinery) |
| **Examples** | Totora reed boats (Lake Titicaca), Yup'ik skin kayaks (Alaska), Swahili dhow traditions |
| **UX** | Coastal/river map layer; weather and safety gating |
| **Extensibility** | Sub-tags: `indigenous_maritime`, `reed`, `wooden_hull` |

### 7. Instrument & Music Craft

| Field | Definition |
|-------|------------|
| **Inclusion** | Instrument making, gamelan, drum carving, violin lineage |
| **Exclusion** | Performance-only bookings without making/learning |
| **Overlap** | Music & Storytelling; Material Craft |
| **Examples** | Cremona violin making, gamelan (Java), ngoma drums (DRC) |
| **UX** | Acoustic/media consent flags; maker-workshop focus |
| **Extensibility** | Sub-tags: `percussion`, `strings`, `wind` |

### 8. Navigation & Wayfinding

| Field | Definition |
|-------|------------|
| **Inclusion** | Pacific wayfinding, star compass knowledge, traditional route literacy |
| **Exclusion** | GPS tourism; generic sailing lessons |
| **Overlap** | Maritime & Watercraft; Land Stewardship (place knowledge) |
| **Examples** | Pacific Island navigation corridors |
| **UX** | Oceanic map projection; elder-led access only |
| **Extensibility** | Sub-tags: `star_navigation`, `coastal_literacy` |

### 9. Music & Storytelling

| Field | Definition |
|-------|------------|
| **Inclusion** | Griot traditions, oral history, ceremonial song, storytelling as transmission |
| **Exclusion** | Entertainment gigs; extractive recording without consent |
| **Overlap** | Textile & Fiber Craft (story quilts); Instrument & Music Craft |
| **Examples** | Griot instrument making (Senegal), intergenerational storytelling (Gee's Bend) |
| **UX** | Recording restrictions; steward-approved media policies |
| **Extensibility** | Sub-tags: `oral_history`, `ceremonial`, `griot` |

---

## Overlap rules

1. **Primary archetype** = dominant transmission mode at the node.  
2. **Secondary archetype** (optional, max 1) recorded in `Notes` until schema v2.  
3. If craft spans two equally, prefer **stewardship-sensitive** archetype for gating.  
4. Indigenous or ritual knowledge → elevate sensitivity before archetype debate.

---

## Legacy label mapping (dataset normalization)

| Legacy (spreadsheet) | Canonical |
|----------------------|-----------|
| Textile Traditions | Textile & Fiber Craft |
| Architectural Craft | Architecture & Building Craft |
| Fermentation & Food | Food & Fermentation |
| Botanical & Medicinal Knowledge | Land Stewardship |
| Metal Craft / Lacquer Craft | Material Craft |

---

## UX implications (atlas, not app yet)

| Layer | Behavior |
|-------|----------|
| **Filter rail** | Multi-select archetypes; AND with corridor |
| **Map overlay** | Color family per archetype; low saturation |
| **Node card** | Archetype badge + craft title + steward type |
| **Application** | Archetype-specific intent questions |
| **Archive** | Media tagged by archetype for longitudinal search |

---

## Future extensibility

- **v2:** Secondary archetype column; sub-tag enum  
- **v3:** Archetype-specific steward review templates  
- **Hard limit:** Do not exceed 12 top-level archetypes without founder council — taxonomy drift erodes map clarity  

**Proposed additions (not approved):** Sacred Ecology, Ritual Art — fold into existing nine via sub-tags until demand proves otherwise.
