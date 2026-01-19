# Contract: Tier 3 Species Entry

**Version**: 1.0
**Applies to**: `universe/bible/species/background/*.md`

## Format Specification

Tier 3 species are grouped by biology type in shared files. Each species entry follows this format:

```markdown
---

**[Species Name]** | [Classification] | [Biology Type]

[1-2 sentence description (25-50 words) covering appearance and notable trait]

*Faction*: [Primary affiliation] | *Human Attitude*: [single word]
```

## File Organization

Group species by biology type:

| File | Biology Types Included |
|------|------------------------|
| `carbon-based.md` | Standard organic, mammalian, reptilian, avian, aquatic, insectoid |
| `silicon-based.md` | Crystalline, mineral, geological |
| `energy-based.md` | Plasma, electromagnetic, photonic |
| `gaseous.md` | Atmospheric, nebular, non-corporeal |
| `symbiotic.md` | Bonded pairs, parasitic/mutualistic, collective |

Each file header:

```markdown
# Background Species: [Biology Category]

Species in this file are Tier 3 (brief reference) entries for scene population and variety.

---
```

## Entry Examples

```markdown
---

**Korvin** | Neutral | Carbon (Avian)

Tall, crane-like beings with metallic feathers that chime when they move. Known for obsessive record-keeping and serving as neutral arbiters in trade disputes.

*Faction*: Horizon Syndicate | *Human Attitude*: Indifferent

---

**Thessik** | Hostile | Silicon

Living crystal formations that communicate through resonant vibrations. Consider organic life to be a temporary contamination of the universe.

*Faction*: Old Guard | *Human Attitude*: Contemptuous

---

**Vael'moth** | Fascinated | Symbiotic

A bonded pair species: small luminescent creatures that inhabit larger crystalline shells. Fascinated by human individuality, which they find philosophically disturbing.

*Faction*: Observers | *Human Attitude*: Curious
```

## Validation Requirements

### Per Entry
- [ ] Name is unique across all species
- [ ] Classification is one of: Hostile, Sympathetic, Neutral, Fascinated, Wildcard
- [ ] Biology type is specified
- [ ] Description is 25-50 words
- [ ] Faction is named
- [ ] Human attitude is single word

### Per File
- [ ] File header present
- [ ] All entries separated by `---`
- [ ] Entries sorted alphabetically within file
- [ ] Minimum 8-10 species per file

### Word Count (per entry)
- **Minimum**: 50 words
- **Maximum**: 100 words
- **Target**: 60-80 words

### Cross-References
- [ ] All species appear in master index
- [ ] Faction names match established factions
- [ ] No duplicate names with Tier 1 or Tier 2 species
