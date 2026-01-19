# Contract: Tier 2 Species Profile

**Version**: 1.0
**Applies to**: `universe/bible/species/recurring/*.md`

## Format Specification

```markdown
# Species Profile: [NAME]

**Classification**: [Hostile|Sympathetic|Neutral|Fascinated|Wildcard]
**Consortium Status**: [Status]
**Population**: ~[X.X] [billion|trillion]
**Primary Territory**: [Territory Name] ([Region])

---

## Designations

- **Formal**: [Official name]
- **Common**: [Name]
- **Self-Designation**: *[native term]* ("[translation]")

---

## Physical Description

[50-100 words describing appearance]

**Key Features**:
- [Primary distinguishing feature]
- [Secondary feature]
- [Optional: third feature]

---

## Cultural Overview

[25-50 words on core cultural trait]

**Core Value**: *[Native term]* ([Translation])

---

## Attitude Toward Humans

**Classification**: [single word]

[25-50 words on why and how]

---

## Notable Individual (optional)

**[Name]**: [1-2 sentences]

---

## Faction Affiliation

- **Primary**: [Faction name]

---

*Word Count: ~[XXX]*
```

## Validation Requirements

### Required Fields
- [ ] Name is unique across all species
- [ ] Classification is one of: Hostile, Sympathetic, Neutral, Fascinated, Wildcard
- [ ] Population uses format: `~X.X [unit]`
- [ ] Physical description includes at least 2 Key Features
- [ ] At least 1 Core Value
- [ ] Human attitude classification and brief explanation
- [ ] Primary faction affiliation

### Word Count
- **Minimum**: 200 words
- **Maximum**: 400 words
- **Target**: 250-350 words

### Cross-References
- [ ] Faction name matches `universe/bible/factions/`
- [ ] Territory name matches established geography
- [ ] Species name appears in master index

### Constitution Compliance
- [ ] Principle I: Maintains tone consistency
- [ ] No contradictions with Tier 1 species lore
