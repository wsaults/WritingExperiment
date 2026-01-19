# Quickstart: Using the Expanded Universe

**Feature**: 002-universe-breadth
**Date**: 2026-01-19

## Overview

This guide explains how to use the expanded universe documentation (~100 species, human culture, enhanced dungeons, items, and geography) when writing scenes for the LitRPG series.

---

## Finding Species for Your Scene

### Step 1: Identify What You Need

| Scene Type | Look For |
|------------|----------|
| Political negotiation | Founders with conflicting interests |
| Market/station crowd | Mix of Tier 2/3 species for variety |
| Combat encounter | Species with warrior archetype |
| Information gathering | Scholar or spy archetype species |
| Ally recruitment | Sympathetic or fascinated species |
| Antagonist | Hostile species or faction-opposed |

### Step 2: Use the Master Index

Location: `universe/bible/species/index.md`

**Quick Lookup Methods**:

1. **Need a specific attitude?** → "By Human Attitude" section
2. **Need a story role?** → "By Narrative Archetype" section
3. **Need visual variety?** → "By Biology Type" section
4. **Need faction alignment?** → "By Faction Affiliation" section
5. **Know the name?** → "Alphabetical Index"

### Step 3: Check Detail Level

| Tier | Use Case | Location |
|------|----------|----------|
| Tier 1 | Named characters, extended scenes | `species/founders/` or `species/major/` |
| Tier 2 | Recurring minor characters | `species/recurring/` |
| Tier 3 | Background, one-line mentions | `species/background/` |

---

## Writing a Multi-Species Scene

### Example: Crowded Station Scene

1. **Open the master index** → "By Biology Type"
2. **Select 5-7 species** from different biology categories for visual variety
3. **Check attitude distribution** → mostly neutral for background, 1-2 interesting attitudes for color
4. **Read their entries** for quick descriptors

**Sample selection**:
- Velthrani (reptilian, hostile) - passing through, dismissive
- Kindari (insectoid, sympathetic) - helping a lost traveler
- [New silicon species] (neutral) - vendor at a stall
- [New avian species] (fascinated) - watching humans curiously
- [New gaseous species] (neutral) - drifting overhead

### Pro Tips

- **Don't over-describe Tier 3 species** - one visual detail is enough
- **Use slang names** for flavor when appropriate
- **Mix attitudes** to create tension even in background
- **Repeat important species** across scenes for continuity

---

## Using Human Culture

### Settlement Types

Location: `universe/culture/human-settlements.md`

| Type | Use When |
|------|----------|
| Fortress Community | Showing human militarization, resource conflicts |
| Nomadic Band | Travel sequences, scavenger encounters |
| Hidden Enclave | Secret meetings, resistance storylines |

### Human Factions

Location: `universe/culture/human-factions.md`

| Faction | Use When |
|---------|----------|
| Might-Makes-Right | Victor scenes, antagonist humans |
| Cooperative Survival | Allies, hope scenes |
| System Exploiters | Information, strategy discussions |
| Resistance/Abolitionists | Ideological conflict, moral debates |

---

## Writing Dungeon Scenes

### Finding Dungeon Details

Location: `universe/plot/book-{N}/dungeon-design.md`

Each dungeon file contains:

1. **Environment** - Setting description, rules, hazards
2. **Monsters** - Categories, behaviors, boss details
3. **Progression** - Entry, milestones, rewards
4. **Integration** - How protagonist's skills apply

### Quick Reference

| Book | Theme | Key Mechanic |
|------|-------|--------------|
| 1 | Industrial/Transition | Optimization pressure |
| 2 | Underwater/Bio-organic | [TBD in expansion] |
| 3 | Social/Political | [TBD in expansion] |
| 4 | Reality-bending | [TBD in expansion] |
| 5 | System-level | [TBD in expansion] |

---

## Writing Shopping/Loot Scenes

### Item Catalog

Location: `universe/mechanics/items/item-catalog.md`

**Format**:
```
**[Item Name]** | [Tier]
*Cost*: [amount] UC
*Effect*: [what it does]
*Flavor*: [narrative description]
```

### Tier Expectations by Book

| Book | Common Tiers Available |
|------|------------------------|
| 1 | Common, Uncommon |
| 2 | Uncommon, Rare |
| 3 | Rare, some Epic |
| 4 | Epic common |
| 5 | Epic, Legendary |

---

## Writing Travel Scenes

### Galactic Geography

Location: `universe/bible/geography/galactic-regions.md`

| Region | Character | Travel Time from Earth |
|--------|-----------|------------------------|
| Core Worlds | Political center | Weeks |
| Third Spiral Confluence | Earth's neighborhood | Local |
| Outer Rim | Frontier, lawless | Months |
| Quarantine Zones | Forbidden | N/A |

### Travel Descriptions

- Reference transit corridors and named stations
- Use relative time ("weeks" not "3.7 days")
- Mention species demographics of destinations

---

## Glossary Integration

Location: `universe/bible/glossary.md`

### Before Writing

1. Check glossary for correct terminology
2. Use established faction names exactly
3. Verify species name spelling

### Adding New Terms

If you introduce a term not in glossary:
1. Add it during editing pass
2. Format: `**[Term]** (pronunciation): [definition]`
3. Include source reference

---

## Constitution Compliance Checklist

Before finalizing any scene:

- [ ] **Tone**: Maintains action-comedy balance
- [ ] **Voice**: Character voices are consistent
- [ ] **Mechanics**: Any game rules match established system
- [ ] **Consistency**: Species behaviors match their profiles
- [ ] **Plot**: Doesn't contradict series arc

---

## File Quick Reference

```
universe/
├── bible/
│   ├── species/
│   │   ├── index.md          ← START HERE for species lookup
│   │   ├── founders/         ← Tier 1 founder species
│   │   ├── major/            ← Tier 1 non-founders
│   │   ├── recurring/        ← Tier 2 species
│   │   └── background/       ← Tier 3 species (by biology)
│   ├── geography/
│   │   └── galactic-regions.md
│   └── glossary.md
├── culture/
│   ├── human-settlements.md
│   └── human-factions.md
├── mechanics/
│   └── items/
│       └── item-catalog.md
└── plot/
    └── book-{N}/
        └── dungeon-design.md
```
