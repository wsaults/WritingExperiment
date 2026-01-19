# Research: Universe Breadth Expansion

**Date**: 2026-01-19
**Feature**: 002-universe-breadth

## Research Summary

This document consolidates research decisions for expanding the universe from 5 species to ~100, completing founder species, and enhancing world documentation.

---

## 1. Existing Species Format Analysis

### Decision: Maintain existing Tier 1 format as canonical

**Rationale**: Existing species files (Velthrani: ~850 words, Kindari: ~870 words) establish a proven structure that covers all required elements.

**Existing Tier 1 Structure**:
```markdown
# Species Profile: [Name]

**Classification**: [Hostile/Sympathetic/Neutral/Fascinated/Wildcard]
**Consortium Status**: [Founder/Observer/Non-voting/etc.]
**Population**: [number]
**Primary Territory**: [region]

## Designations
- Formal, Common, Slang, Self-Designation

## Physical Description
- Height, body type, visual reference notes

## Cultural Overview
- Core values with native terms

## Political Structure

## Relationship to Games/System

## Attitude Toward Humans

## Notable Individuals

## Faction Affiliations

*Word Count: [target]*
```

**Alternatives Considered**:
- Inventing new format → Rejected (inconsistent with existing content)
- Simplified format for all → Rejected (loses detail for important species)

---

## 2. Species Tier System Design

### Decision: Three-tier system with distinct formats

| Tier | Word Count | Count | Purpose | Sections |
|------|------------|-------|---------|----------|
| Tier 1 | 500-1,000 | ~20-22 | Founders + plot-critical | Full format (all sections) |
| Tier 2 | 200-400 | ~30-35 | Recurring, faction-affiliated | Core sections only |
| Tier 3 | 50-100 | ~45-50 | Background variety | Quick reference format |

**Tier 2 Sections** (reduced):
- Classification, Consortium Status, Population, Territory
- Physical Description (brief)
- Cultural Overview (1-2 sentences)
- Attitude Toward Humans
- Notable Individuals (optional, 1 max)
- Faction Affiliations

**Tier 3 Format** (minimal):
```markdown
**[Species Name]** | [Classification] | [Biology Type]
[1-2 sentence description covering appearance and notable trait]
*Faction*: [primary affiliation] | *Human Attitude*: [one word]
```

**Rationale**: Tiered system allows comprehensive coverage without unsustainable word counts. 100 species at Tier 1 = 50,000-100,000 words (impractical). Tiered approach: ~18,500-22,000 words (manageable).

---

## 3. D&D Archetype Mapping to Sci-Fi

### Decision: Adapt 12 biological categories with original names

| D&D Inspiration | Sci-Fi Adaptation | Notes |
|-----------------|-------------------|-------|
| Mind Flayers | **Psychic Manipulators** | Telepathy, memory consumption |
| Hive-Mind (Formians) | **Collective Consciousness** | Beyond Thex—true shared mind |
| Changelings/Doppelgangers | **Polymorphic Species** | Molecular reconfiguration, not magic |
| Elementals | **Energy Beings** | Plasma, electromagnetic, gravitational |
| Dragonborn/Lizardfolk | **Scaled Variants** | Diverse reptilian evolution |
| Formians/Thri-Kreen | **Insectoid Species** | Chitinous, segmented, compound eyes |
| Tritons/Merfolk | **Aquatic Species** | Gill-based, pressure-adapted |
| Aarakocra/Kenku | **Avian Species** | Feathered, hollow-boned, flight-capable |
| Various Mammalian | **Mammalian Variants** | Furred, warm-blooded, viviparous |
| Earth Elementals | **Silicon-Based Life** | Crystal structures, mineral metabolism |
| Air Elementals/Ghosts | **Non-Corporeal Entities** | Gaseous, energy-based consciousness |
| Symbionts | **Symbiotic Pairs** | Two-organism species, interdependent |

**Naming Convention**: No direct D&D references. All species get original names following established patterns:
- 2-3 syllables preferred
- Pronounceable
- Apostrophes used sparingly (1 per name max)
- Pronunciation guide included

**Rationale**: D&D provides structural inspiration but the setting demands originality. "Space Mind Flayers" breaks immersion; original species with similar narrative roles maintains genre while feeling fresh.

---

## 4. Founder Species Requirements

### Decision: 12 founders with distinct political positions

**Political Bloc Structure**:
| Bloc | Species Count | Position |
|------|---------------|----------|
| Velthrani Coalition | 3-4 | Traditional dominance, anti-human |
| Reformist Faction | 2-3 | Moderate change, pragmatic |
| Isolationist | 2-3 | Minimal intervention, focus on own territories |
| Wildcard | 2-3 | Unpredictable, unique agendas |

**Required Coverage**:
- At least 2 founders with reasons to support humans (per spec requirement)
- At least 2 founders with historical conflicts with Velthrani
- All 12 must have distinct visual appearance (no overlap)
- Political positions must enable plot flexibility

**Thirteenth Founder Mystery**:
- All 12 founder histories reference the Compact
- Subtle hints that "something" is missing from records
- No explicit thirteenth founder named or described
- Preserve mystery for series revelation

---

## 5. Existing Species Classification

### Decision: Reclassify existing 5 species

| Species | Current Location | New Location | Tier |
|---------|------------------|--------------|------|
| Velthrani | `species/velthrani.md` | `species/founders/velthrani.md` | 1 |
| Kindari | `species/kindari.md` | `species/major/kindari.md` | 1 |
| Quorathi | `species/quorathi.md` | `species/major/quorathi.md` | 1 |
| Thex Collective | `species/thex-collective.md` | `species/major/thex-collective.md` | 1 |
| Vorrax | `species/vorrax.md` | `species/major/vorrax.md` | 1 |

**Rationale**:
- Velthrani confirmed as founder in existing content
- Others are non-founders but plot-relevant (Tier 1 worthy)
- No content changes needed, just reorganization
- Creates clear directory structure for expansion

---

## 6. Species Distribution by Attitude

### Decision: Balanced distribution across attitudes

| Attitude | Tier 1 | Tier 2 | Tier 3 | Total | % |
|----------|--------|--------|--------|-------|---|
| Hostile | 4-5 | 8-10 | 12-15 | ~25 | 25% |
| Neutral | 5-6 | 10-12 | 18-20 | ~35 | 35% |
| Sympathetic | 3-4 | 6-8 | 8-10 | ~18 | 18% |
| Fascinated | 3-4 | 5-7 | 5-8 | ~15 | 15% |
| Wildcard | 2-3 | 2-3 | 2-3 | ~7 | 7% |

**Rationale**:
- ~40% hostile/neutral creates tension
- ~33% sympathetic/fascinated enables allies and interesting dynamics
- Wildcards provide plot flexibility
- Distribution ensures narrative variety

---

## 7. Species Distribution by Narrative Archetype

### Decision: Cover all common narrative roles

| Archetype | Minimum Species | Notes |
|-----------|-----------------|-------|
| Warrior | 8+ | Combat-focused cultures |
| Merchant | 6+ | Trade-focused, economic power |
| Scholar | 5+ | Knowledge-focused, researchers |
| Healer | 4+ | Medical/support specialists |
| Trickster | 5+ | Deception, manipulation |
| Diplomat | 4+ | Negotiation, alliance-building |
| Spy | 4+ | Information gathering |
| Artisan | 4+ | Crafting, creation-focused |
| Mystic | 3+ | Spiritual, philosophical |
| Outcast | 3+ | Rejected, exile species |

**Rationale**: Ensures any scene requiring a specific character type has multiple species options (spec requirement: 3+ per archetype).

---

## 8. Human Species Entry Approach

### Decision: Write from galactic anthropologist perspective

**Format**: Standard Tier 1 format but inverted perspective
- Physical description emphasizes traits aliens find notable
- Cultural overview highlights behaviors that seem strange to long-lived species
- "Entertainment value factors" section replaces "Relationship to Games"
- Attitude section becomes "Galactic Perception"

**Key Angles**:
- Short lifespan = compressed decision-making (fascinating)
- Emotional transparency = excellent entertainment (valuable)
- Creativity under pressure = novelty generation (rare)
- Pack-bonding tendencies = dramatic relationship dynamics (profitable)
- Stubborn optimism = willingness to fight unwinnable odds (entertaining)

**Rationale**: Provides fresh perspective on humanity while maintaining species file format consistency.

---

## 9. Human Settlement Types

### Decision: Three distinct settlement archetypes

| Type | Governance | Culture | Location |
|------|------------|---------|----------|
| **Fortress Communities** | Military hierarchy | Defensible, strict, resource-controlled | Converted structures (malls, stadiums) |
| **Nomadic Bands** | Consensus/charismatic leader | Mobile, scavenger, flexible | Vehicles, temporary camps |
| **Hidden Enclaves** | Democratic/council | Concealment priority, self-sufficient | Underground, remote, disguised |

**Rationale**: Covers major post-apocalyptic survival strategies while enabling narrative variety. Each type creates different story opportunities.

---

## 10. Human Faction Philosophies

### Decision: Four factions covering philosophical spectrum

| Faction | Philosophy | Leader Type | Relationship to Games |
|---------|------------|-------------|----------------------|
| **Might-Makes-Right** (Victor's) | Strength, hierarchy, dominance | Strongmen | Play to win at any cost |
| **Cooperative Survival** | Mutual aid, shared resources | Council/elected | Survive together or not at all |
| **System Exploiters** | Study and exploit game mechanics | Analysts | Beat the game through knowledge |
| **Resistance/Abolitionists** | Refuse to play, seek escape | Idealists | Reject the games entirely |

**Rationale**: Creates meaningful human political conflict without overshadowing galactic scope. Each faction offers different ally/antagonist potential.

---

## 11. Dungeon Expansion Approach

### Decision: Expand to match Book 1 template structure

**Target Structure** (per dungeon):
- Overview (~200 words)
- Environment: Theme, Aesthetic, Unique Rules (3+), Hazards (4+) (~600 words)
- Monsters: 5 categories + boss encounter + ecology (~600 words)
- Progression: Entry, Milestones, Exit, Rewards (~400 words)
- Integration: Protagonist skills, Challenges, Learnings (~300 words)

**Total Target**: 2,000-2,200 words per dungeon

**Unique Mechanics Requirement**: Each dungeon must have 3+ mechanics not shared with others:
- Book 1: Transition instability, resonance points, optimization pressure
- Book 2: [Underwater-specific mechanics needed]
- Book 3: [Social/political-specific mechanics needed]
- Book 4: [Reality-bending-specific mechanics needed]
- Book 5: [System-level-specific mechanics needed]

---

## 12. Item Catalog Structure

### Decision: Organize by category with tier examples

**Categories**:
- Weapons (5+ examples across tiers)
- Armor/Defense (4+ examples)
- Consumables (6+ examples)
- Tools/Utility (3+ examples)
- Skill Enhancements (2+ examples)

**Format per item**:
```markdown
**[Item Name]** | [Tier: Common/Uncommon/Rare/Epic/Legendary]
*Cost*: [Universal Currency amount]
*Effect*: [mechanical effect]
*Flavor*: [1 sentence narrative description]
```

**Rationale**: 20+ items across categories provides sufficient reference for shopping/loot scenes without exhaustive database.

---

## 13. Galactic Geography Structure

### Decision: Four major regions plus Earth's position

**Regions**:
| Region | Political Control | Character | Travel from Earth |
|--------|-------------------|-----------|-------------------|
| **Core Worlds** | Consortium HQ, founders | Political center, dense | Weeks |
| **Third Spiral Confluence** | Mixed, contested | Earth's neighborhood, frontier | Local |
| **Outer Rim** | Observer species, refugees | Lawless, independent | Months |
| **Quarantine Zones** | None (prohibited) | Dangerous, mysterious | Forbidden |

**Additional Elements**:
- Major transit corridors (named)
- Key stations/hubs (3-4 named locations)
- Travel time scale (relative, not absolute)

**Rationale**: Provides enough geography for travel scenes and political context without requiring detailed star maps.

---

## Research Conclusions

All NEEDS CLARIFICATION items have been resolved. The research establishes:

1. **Species Format**: Three-tier system maintaining existing Tier 1 format
2. **D&D Mapping**: 12 biological categories with original sci-fi names
3. **Founder Politics**: 4 political blocs enabling plot flexibility
4. **File Organization**: Clear directory structure with existing species reclassified
5. **Distribution Balance**: Attitude and archetype coverage ensures narrative variety
6. **Supporting Content**: Human culture, dungeons, items, geography all have clear approaches

**Ready for Phase 1**: Data model and contract generation.
