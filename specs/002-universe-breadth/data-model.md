# Data Model: Universe Breadth Expansion

**Date**: 2026-01-19
**Feature**: 002-universe-breadth

## Entity Overview

```
Species Catalog (~100 entities)
├── Founders (12)           → Tier 1 format
├── Major Species (8-10)    → Tier 1 format
├── Recurring Species (30-35) → Tier 2 format
└── Background Species (45-50) → Tier 3 format

Supporting Content
├── Human Culture
│   ├── Settlements (3 types)
│   └── Factions (4 philosophies)
├── Dungeon Expansions (4 books)
├── Item Catalog (20+ items)
└── Galactic Geography (4 regions)

Index & Reference
└── Species Master Index (6 taxonomies)
```

---

## Species Entity Model

### Tier 1 Species (Detailed)

**Entity**: `SpeciesTier1`
**Location**: `universe/bible/species/founders/` or `universe/bible/species/major/`
**Format**: Markdown file
**Word Count**: 500-1,000

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `name` | string | YES | Species name (2-3 syllables, pronounceable) |
| `classification` | enum | YES | Hostile, Sympathetic, Neutral, Fascinated, Wildcard |
| `consortium_status` | string | YES | Founder, Observer, Non-voting, etc. |
| `population` | string | YES | Approximate count with scale indicator |
| `primary_territory` | string | YES | Region name and descriptor |
| `designations.formal` | string | YES | Official name |
| `designations.common` | string | YES | Common usage name |
| `designations.slang` | string | YES | Derogatory/informal names |
| `designations.self` | string | YES | What they call themselves |
| `physical_description` | text | YES | 100-200 words with visual reference notes |
| `cultural_overview` | text | YES | 100-200 words with core values |
| `political_structure` | text | YES | 50-100 words |
| `relationship_to_games` | text | YES | 75-150 words |
| `attitude_toward_humans` | text | YES | 75-150 words |
| `notable_individuals` | list | YES | 2-3 named individuals |
| `faction_affiliations` | list | YES | Primary, Secondary, Opposed |

**Validation Rules**:
- Name must be unique across all species
- Classification must be one of 5 enum values
- Population format: `~X.X [unit]` (billion, trillion, etc.)
- Notable individuals must have names and brief descriptions
- Faction affiliations must reference existing factions

---

### Tier 2 Species (Standard)

**Entity**: `SpeciesTier2`
**Location**: `universe/bible/species/recurring/`
**Format**: Markdown file
**Word Count**: 200-400

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `name` | string | YES | Species name |
| `classification` | enum | YES | Same enum as Tier 1 |
| `consortium_status` | string | YES | Status designation |
| `population` | string | YES | Approximate count |
| `primary_territory` | string | YES | Region name |
| `physical_description` | text | YES | 50-100 words |
| `cultural_overview` | text | YES | 25-50 words |
| `attitude_toward_humans` | text | YES | 25-50 words |
| `notable_individuals` | list | NO | 0-1 named individual |
| `faction_affiliations` | list | YES | Primary affiliation only |

**Validation Rules**:
- Same uniqueness requirement as Tier 1
- Abbreviated sections must still be complete

---

### Tier 3 Species (Brief)

**Entity**: `SpeciesTier3`
**Location**: `universe/bible/species/background/`
**Format**: Markdown file (multiple species per file, grouped by biology)
**Word Count**: 50-100 per species

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `name` | string | YES | Species name |
| `classification` | enum | YES | Single word classification |
| `biology_type` | enum | YES | Carbon, Silicon, Energy, Gaseous, Symbiotic |
| `description` | text | YES | 1-2 sentences (25-50 words) |
| `faction` | string | YES | Primary affiliation |
| `human_attitude` | string | YES | Single word (hostile, neutral, etc.) |

**Grouping**: Tier 3 species grouped by biology type in shared files:
- `background/carbon-based.md`
- `background/silicon-based.md`
- `background/energy-based.md`
- `background/gaseous.md`
- `background/symbiotic.md`

---

### Species Master Index

**Entity**: `SpeciesIndex`
**Location**: `universe/bible/species/index.md`
**Format**: Multi-table Markdown

**Taxonomies** (6 views):

1. **Alphabetical**: All species A-Z with tier indicator
2. **Founder Status**: Founders | Non-Founders
3. **Faction Affiliation**: Grouped by primary faction
4. **Human Attitude**: Hostile | Neutral | Sympathetic | Fascinated | Wildcard
5. **Narrative Archetype**: Warrior | Merchant | Scholar | Healer | Trickster | Diplomat | Spy | Artisan | Mystic | Outcast
6. **Biology Type**: Carbon | Silicon | Energy | Gaseous | Symbiotic

Each entry includes: Name, Tier, File Link

---

## Human Culture Entities

### Settlement Type

**Entity**: `HumanSettlement`
**Location**: `universe/culture/human-settlements.md`

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `name` | string | YES | Settlement type name |
| `governance` | string | YES | Leadership structure |
| `culture` | text | YES | 100-150 words on values, lifestyle |
| `typical_locations` | list | YES | 3-5 example locations |
| `survival_strategy` | text | YES | 50-100 words on how they survive |
| `relationship_to_games` | text | YES | How they interact with game mechanics |
| `example_settlement` | object | NO | Named example with details |

**Defined Types**:
1. Fortress Communities
2. Nomadic Bands
3. Hidden Enclaves

---

### Human Faction

**Entity**: `HumanFaction`
**Location**: `universe/culture/human-factions.md`

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `name` | string | YES | Faction name |
| `philosophy` | text | YES | 75-100 words on core beliefs |
| `leader_type` | string | YES | Type of leadership |
| `game_stance` | text | YES | 50-75 words on relationship to games |
| `notable_adherents` | list | NO | Named characters who follow this philosophy |
| `conflicts_with` | list | YES | Other factions they oppose |

**Defined Factions**:
1. Might-Makes-Right (Victor's faction)
2. Cooperative Survival
3. System Exploiters
4. Resistance/Abolitionists

---

## Dungeon Entity

**Entity**: `DungeonDesign`
**Location**: `universe/plot/book-{N}/dungeon-design.md`

| Section | Required | Word Target |
|---------|----------|-------------|
| Overview | YES | 200 |
| Environment.Theme | YES | 100 |
| Environment.UniqueRules | YES | 200 (3+ rules) |
| Environment.Hazards | YES | 200 (4+ hazards) |
| Monsters.Categories | YES | 300 (5 categories) |
| Monsters.BossEncounter | YES | 200 |
| Monsters.Ecology | YES | 100 |
| Progression.Entry | YES | 75 |
| Progression.Milestones | YES | 150 |
| Progression.Exit | YES | 75 |
| Progression.Rewards | YES | 100 |
| Integration.Skills | YES | 100 |
| Integration.Challenges | YES | 100 |
| Integration.Learnings | YES | 100 |

**Total Target**: 2,000+ words per dungeon

---

## Item Entity

**Entity**: `Item`
**Location**: `universe/mechanics/items/item-catalog.md`

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `name` | string | YES | Item name |
| `tier` | enum | YES | Common, Uncommon, Rare, Epic, Legendary |
| `category` | enum | YES | Weapon, Armor, Consumable, Tool, Enhancement |
| `cost` | number | YES | Universal Currency value |
| `effect` | text | YES | Mechanical effect (25-50 words) |
| `flavor` | text | YES | Narrative description (1 sentence) |

**Distribution Requirement**: 20+ items covering all tiers and categories

---

## Geography Entity

**Entity**: `GalacticRegion`
**Location**: `universe/bible/geography/galactic-regions.md`

| Field | Type | Required | Description |
|-------|------|----------|-------------|
| `name` | string | YES | Region name |
| `political_control` | text | YES | Who controls/influences |
| `character` | text | YES | 50-75 words on what it's like |
| `travel_from_earth` | string | YES | Relative travel time |
| `key_locations` | list | NO | Named stations, hubs, etc. |
| `species_demographics` | text | NO | Who lives there |

**Defined Regions**:
1. Core Worlds
2. Third Spiral Confluence
3. Outer Rim
4. Quarantine Zones

---

## Relationships

```
Species ─────┬───── belongs_to ─────> Faction
             │
             ├───── has_attitude_toward ─────> Humans
             │
             └───── indexed_by ─────> SpeciesIndex

HumanFaction ───── conflicts_with ───── HumanFaction

DungeonDesign ───── challenges ───── Protagonist (skills)

Item ───── available_at ───── DungeonShop

GalacticRegion ───── controlled_by ───── Faction
```

---

## State Transitions

### Species Attitude (can change across series)

```
HOSTILE ──────> NEUTRAL ──────> SYMPATHETIC
    ↑               ↑               ↓
    └───────────────┴───── FASCINATED
                            ↓
                        WILDCARD (any transition)
```

### Item Tier Progression (per book)

```
Book 1: Common → Uncommon
Book 2: Uncommon → Rare
Book 3: Rare common, Epic introduced
Book 4: Epic common, Legendary teased
Book 5: Legendary available
```

---

## File Naming Conventions

| Entity Type | Pattern | Example |
|-------------|---------|---------|
| Tier 1 Species | `{species-name}.md` | `velthrani.md` |
| Tier 2 Species | `{species-name}.md` | `korinth.md` |
| Tier 3 Species | `{biology-type}.md` | `carbon-based.md` |
| Human Culture | `human-{topic}.md` | `human-settlements.md` |
| Dungeon Design | `dungeon-design.md` | (per book directory) |
| Items | `item-catalog.md` | (single file) |
| Geography | `galactic-regions.md` | (single file) |

---

## Glossary Integration

All new content must use terms from `universe/bible/glossary.md`. New terms to be added:

- Species names (all ~100)
- Settlement type names
- Human faction names
- New dungeon-specific terminology
- Item names (notable ones)
- Region names

Format for glossary entries:
```markdown
**[Term]** (pronunciation): [definition]. *Source*: [file reference]
```
