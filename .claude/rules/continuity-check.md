# Continuity Check Rules

**Applies to**: All prose generation, character references, world-building details

## The Cardinal Rule

**Never contradict established canon.** The universe bible, character files, and previous chapters are authoritative. When in doubt, verify before writing.

---

## Pre-Writing Verification Workflow

### Before Writing Any Scene

**Step 1: Identify what you're referencing**
- Which characters appear?
- Which locations are mentioned?
- Which game mechanics are used?
- Which species/factions are involved?

**Step 2: Consult required documents**

| Element | Required Check |
|---------|----------------|
| Protagonist action/thought | `universe/characters/protagonist.md` |
| Named character | `universe/characters/{type}/{name}.md` |
| Species behavior | `universe/bible/species/{name}.md` |
| Faction politics | `universe/bible/factions/{name}.md` |
| Game mechanic | `universe/mechanics/{relevant-file}.md` |
| Established location | `universe/bible/geography/` or plot docs |
| Previous events | Earlier chapters in current book |

**Step 3: Note specific details**
- Exact stat values if referenced
- Character quirks/speech patterns
- Established relationships
- Prior injuries/conditions
- Timeline position

---

## Mandatory Cross-References

### Character Consistency

**Always verify before writing a character**:
- [ ] Name spelled correctly (including apostrophes for alien names)
- [ ] Physical description matches established profile
- [ ] Speech patterns align with voice documentation
- [ ] Current status (alive, injured, location) matches last appearance
- [ ] Relationships with other characters are accurate

**For the protagonist specifically**:
- [ ] Current level matches progression
- [ ] Skills mentioned exist and work as documented
- [ ] Stats referenced are accurate
- [ ] Inventory items are actually possessed
- [ ] Voice matches current book's arc position

### World Consistency

**Always verify before world-building**:
- [ ] Species names and characteristics match bible
- [ ] Faction positions align with established politics
- [ ] Technology/magic rules follow mechanics docs
- [ ] Geography references match established locations
- [ ] Timeline fits series chronology

### Mechanics Consistency

**Always verify before using game elements**:
- [ ] Skill names match `universe/mechanics/skills.md`
- [ ] Stat abbreviations are correct (STR, AGI, etc.)
- [ ] Level-appropriate abilities (no using skills not yet learned)
- [ ] Currency/economy follows `universe/mechanics/economy.md`
- [ ] System interface format matches established style

---

## Contradiction Detection

### Red Flags to Watch For

**Character contradictions**:
- Referencing events the character wasn't present for
- Using abilities the character doesn't have
- Personality shifts without narrative justification
- Physical descriptions that don't match

**World contradictions**:
- Species behaving against established nature
- Factions taking positions contrary to their philosophy
- Technology doing things it shouldn't
- Geography that doesn't match established maps

**Mechanics contradictions**:
- Stats that don't add up
- Skills working differently than documented
- Economy values that break established scale
- Progression that skips established requirements

### When You Find an Inconsistency

**If the inconsistency is in YOUR draft**:
1. Fix it immediately
2. Verify the fix against source documents
3. Check if the error propagated elsewhere

**If the inconsistency is in EXISTING canon**:
1. Do NOT silently "fix" it in your writing
2. Flag for human review: "Note: Potential inconsistency found between X and Y"
3. Use the more established/important source as authoritative
4. Document the discrepancy for later resolution

---

## Scene-Specific Checklists

### Combat Scenes
- [ ] Character's current health/status from previous scene
- [ ] Available skills and their cooldowns
- [ ] Equipped items and inventory
- [ ] Environmental details match location
- [ ] Enemy types consistent with area/dungeon

### Dialogue Scenes
- [ ] All speakers' names verified
- [ ] Relationship history between speakers acknowledged
- [ ] Information characters have vs. don't have respected
- [ ] Speech patterns match character profiles

### Exploration Scenes
- [ ] Location details match established descriptions
- [ ] Dungeon rules consistent with dungeon-design.md
- [ ] Flora/fauna appropriate to environment
- [ ] Previous discoveries in this area acknowledged

### Flashback/Memory Scenes
- [ ] Timeline accuracy verified
- [ ] Characters' past states (younger, different circumstances)
- [ ] Events match established backstory
- [ ] No anachronistic references

---

## Quick Reference: File Locations

```
universe/
├── bible/
│   ├── species/          # All species profiles
│   ├── factions/         # Faction details
│   ├── geography/        # Location information
│   ├── cosmology.md      # Universe rules
│   ├── history.md        # Timeline
│   └── glossary.md       # Terminology
├── characters/
│   ├── protagonist.md    # Marcus Reeves
│   ├── companions/       # Allied characters
│   ├── antagonists/      # Enemy characters
│   └── supporting/       # Minor characters
├── mechanics/
│   ├── stats.md          # Stat system
│   ├── skills.md         # Skill details
│   ├── classes.md        # Class system
│   ├── economy.md        # Currency/items
│   └── system-rules.md   # System behavior
├── style/
│   ├── voice-guide.md    # Protagonist voice
│   ├── tone-guide.md     # Tone balance
│   └── prose-examples.md # Writing templates
└── plot/
    ├── series-arc.md     # Overall story
    └── book-{n}/         # Per-book details
```

---

## The "I'm Not Sure" Protocol

When uncertain about canon:

1. **Search first**: Use grep/find to locate relevant references
2. **Check glossary**: `universe/bible/glossary.md` for terminology
3. **Consult multiple sources**: Cross-reference between files
4. **When truly ambiguous**: Write conservatively (avoid specific claims) and flag for review
5. **Never invent**: Don't create new canon to fill gaps without flagging it

---

*Word Count: ~900*
