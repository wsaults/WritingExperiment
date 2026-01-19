# Contract: Tier 1 Species Profile

**Version**: 1.0
**Applies to**: `universe/bible/species/founders/*.md`, `universe/bible/species/major/*.md`

## Format Specification

```markdown
# Species Profile: [NAME]

**Classification**: [Hostile|Sympathetic|Neutral|Fascinated|Wildcard]
**Consortium Status**: [Founding Species (N of 12)|Observer Species|Non-voting|etc.]
**Population**: ~[X.X] [billion|trillion]
**Primary Territory**: [Territory Name] ([Region])

---

## Designations

- **Formal**: [Official name]
- **Common**: [Name], "[Nickname]"
- **Slang**: [Derogatory terms, comma-separated]
- **Self-Designation**: *[native term]* ("[translation]")

---

## Physical Description

[100-200 words describing appearance]

**Visual Reference Notes**:
- Body type: [description]
- [Feature]: [description]
- [Feature]: [description]
- [Additional features as needed]

[Optional: 1-2 sentences on notable physical capabilities]

---

## Cultural Overview

[100-150 words describing society and values]

**Core Values**:
- *[Native term]* ([Translation]): [explanation]
- *[Native term]* ([Translation]): [explanation]
- *[Native term]* ([Translation]): [explanation]

[Optional: 1-2 sentences on how they view other species]

---

## Political Structure

[50-100 words on governance, leadership, decision-making]

---

## Relationship to Games/System

[75-150 words on how they interact with the entertainment system]

---

## Attitude Toward Humans

**Classification**: [Hostile|Sympathetic|Neutral|Fascinated|Wildcard]/[Secondary descriptor]

[75-150 words explaining why they feel this way and how it manifests]

---

## Notable Individuals

**[Name]** ([Epithet]): [2-3 sentences on role and relevance]

**[Name]** ([Epithet]): [2-3 sentences on role and relevance]

**[Name]** ([Epithet]): [2-3 sentences on role and relevance]

---

## Faction Affiliations

- **Primary**: [Faction name] ([brief descriptor])
- **Secondary**: [Faction name] ([brief descriptor])
- **Opposed**: [Faction name] ([brief descriptor])
- **Complicated**: [Faction name] ([brief descriptor])

[1-2 sentences on general political stance]

---

*Word Count: ~[XXX]*
```

## Validation Requirements

### Required Fields
- [ ] Name is unique across all species
- [ ] Classification is one of: Hostile, Sympathetic, Neutral, Fascinated, Wildcard
- [ ] Population uses format: `~X.X [unit]`
- [ ] At least 3 designations (Formal, Common, Self)
- [ ] Physical description includes Visual Reference Notes
- [ ] At least 3 Core Values with native terms
- [ ] Political structure is defined
- [ ] Games/System relationship is explained
- [ ] Human attitude has classification and explanation
- [ ] At least 2 Notable Individuals
- [ ] At least 3 Faction Affiliations

### Word Count
- **Minimum**: 500 words
- **Maximum**: 1,000 words
- **Target**: 750-850 words

### Cross-References
- [ ] Faction names match `universe/bible/factions/`
- [ ] Territory names match `universe/bible/geography/galactic-regions.md`
- [ ] All terms appear in `universe/bible/glossary.md`

### Constitution Compliance
- [ ] Principle I: Descriptions maintain action-comedy tone
- [ ] Principle V: Any game mechanics are consistent with established rules
- [ ] Principle VI: Founder species support series plot architecture
