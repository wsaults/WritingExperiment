# Contract: Species Master Index

**Version**: 1.0
**Applies to**: `universe/bible/species/index.md`

## Format Specification

```markdown
# Species Master Index

**Total Species**: [count]
**Last Updated**: [date]

Quick navigation to species by various taxonomies.

---

## Alphabetical Index

| Species | Tier | Classification | File |
|---------|------|----------------|------|
| [Name] | [1/2/3] | [Classification] | [relative path] |
| ... | ... | ... | ... |

---

## By Founder Status

### Founding Species (12)

| Species | Classification | Territory |
|---------|----------------|-----------|
| [Name] | [Classification] | [Territory] |
| ... | ... | ... |

### Major Non-Founder Species (Tier 1)

| Species | Classification | Territory |
|---------|----------------|-----------|
| [Name] | [Classification] | [Territory] |
| ... | ... | ... |

### Recurring Species (Tier 2)

| Species | Classification | Faction |
|---------|----------------|---------|
| [Name] | [Classification] | [Faction] |
| ... | ... | ... |

### Background Species (Tier 3)

[Link to grouped files by biology type]

---

## By Faction Affiliation

### Old Guard

| Species | Tier | Role |
|---------|------|------|
| ... | ... | ... |

### Liberation Collective

| Species | Tier | Role |
|---------|------|------|
| ... | ... | ... |

### Horizon Syndicate

| Species | Tier | Role |
|---------|------|------|
| ... | ... | ... |

### Observers

| Species | Tier | Role |
|---------|------|------|
| ... | ... | ... |

### Unaffiliated

| Species | Tier | Notes |
|---------|------|-------|
| ... | ... | ... |

---

## By Human Attitude

### Hostile

| Species | Tier | Reason |
|---------|------|--------|
| ... | ... | [brief] |

### Neutral

| Species | Tier | Notes |
|---------|------|-------|
| ... | ... | ... |

### Sympathetic

| Species | Tier | Reason |
|---------|------|--------|
| ... | ... | [brief] |

### Fascinated

| Species | Tier | Interest |
|---------|------|----------|
| ... | ... | [brief] |

### Wildcard

| Species | Tier | Notes |
|---------|------|-------|
| ... | ... | ... |

---

## By Narrative Archetype

Use this index when casting species for specific story roles.

### Warrior Species

| Species | Tier | Combat Style |
|---------|------|--------------|
| ... | ... | ... |

### Merchant Species

| Species | Tier | Trade Specialty |
|---------|------|-----------------|
| ... | ... | ... |

### Scholar Species

| Species | Tier | Knowledge Domain |
|---------|------|------------------|
| ... | ... | ... |

### Healer Species

| Species | Tier | Method |
|---------|------|--------|
| ... | ... | ... |

### Trickster Species

| Species | Tier | Approach |
|---------|------|----------|
| ... | ... | ... |

### Diplomat Species

| Species | Tier | Style |
|---------|------|-------|
| ... | ... | ... |

### Spy Species

| Species | Tier | Specialty |
|---------|------|-----------|
| ... | ... | ... |

### Artisan Species

| Species | Tier | Craft |
|---------|------|-------|
| ... | ... | ... |

### Mystic Species

| Species | Tier | Focus |
|---------|------|-------|
| ... | ... | ... |

### Outcast Species

| Species | Tier | Reason |
|---------|------|--------|
| ... | ... | ... |

---

## By Biology Type

### Carbon-Based (Organic)

| Species | Tier | Subtype |
|---------|------|---------|
| ... | ... | Mammalian/Reptilian/Avian/etc. |

### Silicon-Based

| Species | Tier | Notes |
|---------|------|-------|
| ... | ... | ... |

### Energy-Based

| Species | Tier | Energy Type |
|---------|------|-------------|
| ... | ... | Plasma/EM/Photonic |

### Gaseous/Non-Corporeal

| Species | Tier | Notes |
|---------|------|-------|
| ... | ... | ... |

### Symbiotic

| Species | Tier | Relationship Type |
|---------|------|-------------------|
| ... | ... | Mutualistic/Parasitic/etc. |

---

## Quick Stats

| Category | Count |
|----------|-------|
| Total Species | [N] |
| Tier 1 (Detailed) | [N] |
| Tier 2 (Standard) | [N] |
| Tier 3 (Brief) | [N] |
| Founders | 12 |
| Hostile to Humans | [N] |
| Sympathetic to Humans | [N] |
```

## Validation Requirements

### Completeness
- [ ] All ~100 species appear in Alphabetical Index
- [ ] Every species appears in exactly one founder status category
- [ ] Every species appears in at least one faction affiliation
- [ ] Every species appears in exactly one human attitude category
- [ ] Every species appears in at least one narrative archetype
- [ ] Every species appears in exactly one biology type

### Consistency
- [ ] Tier values match actual file locations
- [ ] Classification values match species file content
- [ ] File paths are valid and relative
- [ ] No duplicate entries in any index

### Coverage Requirements (from spec)
- [ ] 3+ species per narrative archetype (warrior, merchant, scholar, healer, trickster, diplomat, spy minimum)
- [ ] Representatives of all 12 D&D-inspired biology categories
- [ ] Balanced distribution across human attitudes (~25% hostile, ~35% neutral, ~18% sympathetic, ~15% fascinated, ~7% wildcard)

### Maintenance
- [ ] Total Species count matches actual content
- [ ] Last Updated reflects most recent species addition
- [ ] Quick Stats section totals are accurate
