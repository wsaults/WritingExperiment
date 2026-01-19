# Scene Research Workflow

**Applies to**: Pre-writing preparation, document consultation, reference gathering

## The Research Principle

**Write from knowledge, not assumption.** Every scene draws from established canon. Before writing, know what you're working with.

---

## Scene Type Reference Matrix

### What to Read Before Writing Each Scene Type

| Scene Type | Required Reading | Optional Depth |
|------------|------------------|----------------|
| **Combat** | `mechanics/skills.md`, `mechanics/stats.md`, current character state | Dungeon-specific rules, enemy profiles |
| **Dialogue (humans)** | Relevant character files in `characters/` | Previous interactions, relationship history |
| **Dialogue (aliens)** | Species profile in `bible/species/`, faction file if applicable | Cultural details, political context |
| **Dungeon exploration** | `plot/book-{n}/dungeon-design.md` | Environmental hazards, reward structure |
| **Political/faction** | `bible/factions/` for all relevant factions | `bible/history.md` for context |
| **Flashback** | `characters/protagonist.md` backstory section | Timeline verification in `bible/history.md` |
| **Level up/progression** | `mechanics/stats.md`, `mechanics/classes.md`, `mechanics/skills.md` | Build trajectory planning |
| **Shopping/economy** | `mechanics/economy.md`, `mechanics/items/item-catalog.md` | Current inventory state |
| **Travel/geography** | `bible/geography/galactic-regions.md` | Species demographics of destination |
| **System interaction** | `mechanics/system-rules.md` | `style/prose-examples.md` for format |

---

## Pre-Scene Checklist

### 1. Identify Scene Elements

Before writing, list:
- [ ] Characters present (by name)
- [ ] Location (specific)
- [ ] Time in story (chapter/book position)
- [ ] Primary purpose (what does this scene accomplish?)
- [ ] Mechanics involved (skills, items, game elements)

### 2. Gather References

For each element, pull the relevant document:

**Characters**:
```
universe/characters/{type}/{name}.md
```
Note: Current emotional state, last significant event, relevant relationships

**Location**:
```
universe/bible/geography/ OR
universe/plot/book-{n}/dungeon-design.md
```
Note: Environmental details, dangers, atmosphere

**Mechanics**:
```
universe/mechanics/{relevant-system}.md
```
Note: Exact names, effects, limitations

### 3. Verify Continuity

Check against previous scenes:
- What state were characters in when we last saw them?
- What information do they have/lack?
- What items/resources do they possess?
- What promises/setups need payoff?

### 4. Note Key Constraints

Write down (before drafting):
- Hard limits (can't use skill X, character Y isn't here)
- Required elements (must reference Z, setup for later)
- Tone target (action-heavy, dialogue-focused, etc.)

---

## Document Quick-Reference Guide

### Universe Bible (`universe/bible/`)

| File | Contains | Use When |
|------|----------|----------|
| `cosmology.md` | Universe rules, System origin | Writing about how things work |
| `history.md` | Timeline, major events | Flashbacks, faction history, context |
| `glossary.md` | Terminology, names, definitions | Verifying correct terms |
| `species/*.md` | Individual species profiles | Any scene with non-humans |
| `factions/*.md` | Political entities | Political scenes, faction interactions |
| `geography/*.md` | Locations, regions, travel | Travel scenes, location descriptions |

### Characters (`universe/characters/`)

| File | Contains | Use When |
|------|----------|----------|
| `protagonist.md` | Marcus Reeves full profile | Every scene (voice, state, capabilities) |
| `companions/*.md` | Allied character profiles | Scenes with specific companions |
| `antagonists/*.md` | Enemy character profiles | Confrontation scenes |
| `supporting/*.md` | Minor character profiles | When they appear |

### Mechanics (`universe/mechanics/`)

| File | Contains | Use When |
|------|----------|----------|
| `stats.md` | Stat system, values, effects | Any stat reference |
| `skills.md` | Skill names, effects, requirements | Combat, ability use |
| `classes.md` | Class system, progressions | Class discussions, builds |
| `economy.md` | Currency, pricing, trade | Shopping, loot, crafting |
| `system-rules.md` | System behavior, personality | System messages, interface |
| `items/item-catalog.md` | Equipment, consumables | Loot, inventory, purchases |

### Style (`universe/style/`)

| File | Contains | Use When |
|------|----------|----------|
| `voice-guide.md` | Marcus's voice, samples | Checking protagonist voice |
| `tone-guide.md` | Action-comedy balance | Tone calibration |
| `prose-examples.md` | Annotated templates | Structural reference |

### Plot (`universe/plot/`)

| File | Contains | Use When |
|------|----------|----------|
| `series-arc.md` | Overall story, mysteries | Long-term setup/payoff |
| `book-{n}/outline.md` | Per-book plot | Current book structure |
| `book-{n}/dungeon-design.md` | Dungeon specifics | Dungeon scenes |
| `book-{n}/character-introductions.md` | When characters appear | New character scenes |

---

## Research Depth Levels

### Level 1: Quick Reference (Most Scenes)

- Skim relevant character files for current state
- Verify terminology in glossary
- Check one key mechanic if used

**Time**: 2-5 minutes

### Level 2: Standard Preparation (Complex Scenes)

- Read full character profiles for all major characters in scene
- Review location/dungeon documentation
- Cross-reference mechanics being used
- Check previous chapter for continuity

**Time**: 10-15 minutes

### Level 3: Deep Dive (Critical Scenes)

- Full read of all relevant documentation
- Timeline verification against history
- Multiple cross-references for consistency
- Review similar scenes in prose-examples.md

**Time**: 20-30 minutes

**Use Level 3 for**: Major reveals, character deaths, significant progression moments, first encounters with important elements

---

## The "Don't Know" Protocol

When you can't find information in existing docs:

1. **Search thoroughly**: Use grep/find across all docs
2. **Check glossary**: Term might be defined there
3. **Check adjacent files**: Related content might have the answer
4. **Infer conservatively**: Make minimal assumptions based on established patterns
5. **Flag uncertainty**: Note that this detail isn't established: "[Note: Character's hometown not specified in docs]"
6. **Don't invent major canon**: New significant details need human approval

### What You Can Invent Without Flagging

- Minor environmental details (the room had a window)
- Incidental NPC names (the vendor's name was Krix)
- Logical extrapolations (if X is true, Y follows)
- Atmospheric details (the dungeon smelled of copper)

### What Requires Flagging

- Character backstory details not in profile
- New species or faction information
- Mechanical rules not documented
- Historical events not in timeline
- Significant locations not in geography

---

## Post-Research Notes Template

Before writing, create a brief note:

```
Scene: [Brief description]
Characters: [List with current states]
Location: [Name, key details]
Mechanics: [Any game elements being used]
Continuity: [What carries forward from previous scenes]
Required beats: [What must happen]
Constraints: [What can't happen]
Reference files used: [List for later verification]
```

This note becomes your writing anchor and post-draft verification checklist.

---

*Word Count: ~1,100*
