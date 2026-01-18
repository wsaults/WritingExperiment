# Quickstart: LitRPG Universe Planning Documents

**Branch**: `001-litrpg-universe` | **Date**: 2026-01-17

---

## What This Project Produces

This planning phase creates the foundation documents for a 5-novel LitRPG series. You will NOT write prose fiction here—you will create the reference materials that enable consistent, high-quality prose writing later.

### Deliverables Overview

| Deliverable | Purpose | Location |
|-------------|---------|----------|
| Universe Bible | World-building reference | `universe/bible/` |
| Character Bible | Character reference | `universe/characters/` |
| Plot Outlines | Story structure | `universe/plot/` |
| Mechanics System | LitRPG rules | `universe/mechanics/` |
| Style Guide | Writing consistency | `universe/style/` |

---

## How to Use These Documents

### 1. Start with the Constitution

**File**: `.specify/memory/constitution.md`

This is your creative north star. Before making ANY major decision, verify it against the 7 principles:

1. **Action-Comedy Tone** (NON-NEGOTIABLE)
2. Character Voice Consistency
3. Protagonist Identity
4. World Structure: Standalone Dungeons
5. Game Mechanics Integrity
6. Plot Architecture
7. Authenticity Over Trend-Chasing

If a decision conflicts with a principle, either reject the decision or amend the constitution.

### 2. Follow the Data Model

**File**: `specs/001-litrpg-universe/data-model.md`

This defines the STRUCTURE of all your content. When creating any entity (species, faction, character, dungeon), use the schema defined here to ensure completeness.

### 3. Meet the Contracts

**Directory**: `specs/001-litrpg-universe/contracts/`

Each contract specifies EXACTLY what a deliverable must contain. Use these as checklists during creation:

- `universe-bible.md` → Requirements for `universe/bible/`
- `character-bible.md` → Requirements for `universe/characters/`
- `plot-outline.md` → Requirements for `universe/plot/`
- `mechanics-system.md` → Requirements for `universe/mechanics/`
- `style-guide.md` → Requirements for `universe/style/`

### 4. Create Content in Order

**Recommended sequence**:

```
1. Universe Bible (cosmology first—establishes rules)
   └── Species profiles
   └── Faction profiles
   └── History
   └── Glossary

2. Mechanics System (before characters—defines their capabilities)
   └── System rules
   └── Stats
   └── Classes
   └── Skills
   └── Economy

3. Character Bible (after mechanics—can reference system)
   └── Protagonist (FIRST—most important)
   └── Companions
   └── Antagonists
   └── Supporting cast

4. Plot Outlines (after characters and world—can reference everything)
   └── Series arc
   └── Book 1 (detailed)
   └── Books 2-5 (progressively less detailed for now)

5. Style Guide (after character voice is defined)
   └── Voice samples from protagonist work
   └── Tone calibration
   └── Prose examples
```

---

## Validation Process

### After Each Document

1. Check against relevant contract requirements
2. Verify no constitution violations
3. Cross-reference with existing documents
4. Update glossary if new terms introduced

### After Each Category

Run these checks:

**Universe Bible Complete?**
- [ ] Cosmology explains game system origin
- [ ] 5+ species with distinct attitudes
- [ ] 4+ factions with distinct philosophies
- [ ] History seeds mysteries for later books
- [ ] Glossary covers all new terms

**Mechanics Complete?**
- [ ] Stats are defined and balanced
- [ ] Classes include protagonist's path
- [ ] Skills progress logically
- [ ] Economy prevents "too rich" problem
- [ ] System has consistent personality

**Characters Complete?**
- [ ] Protagonist has 15+ voice samples
- [ ] Each companion has independent goals
- [ ] Antagonists escalate across series
- [ ] All major characters have differentiated voices

**Plot Complete?**
- [ ] Series arc has clear escalation
- [ ] Each book has standalone satisfaction
- [ ] Mysteries are planted and will pay off
- [ ] Dungeons are thematically distinct

**Style Complete?**
- [ ] Voice guide captures protagonist authentically
- [ ] Tone guide prevents drift toward grimdark
- [ ] Prose examples cover major scene types

---

## Common Pitfalls to Avoid

### World-Building

- **Don't**: Create more than you need
- **Do**: Create what supports the story

### Character Design

- **Don't**: Make protagonist competent at everything
- **Do**: Define specific expertise (SWE/Robotics) and specific weaknesses

### Mechanics

- **Don't**: Over-engineer the system
- **Do**: Create enough for readers to theorize, not more

### Plot

- **Don't**: Plant mysteries without planned answers
- **Do**: Track every mystery in the Mystery Budget table

### Style

- **Don't**: Write prose before voice is locked
- **Do**: Create samples and validate tone first

---

## Next Steps After Planning

Once all deliverables are complete and validated:

1. Run `/speckit.tasks` to generate implementation task list
2. Begin creating actual content documents in `universe/` directory
3. Validate each document against contracts
4. Proceed to prose drafting (out of scope for this phase)

---

## Quick Reference

### Key Files

| Need | File |
|------|------|
| Creative principles | `.specify/memory/constitution.md` |
| Entity schemas | `specs/001-litrpg-universe/data-model.md` |
| Spec requirements | `specs/001-litrpg-universe/spec.md` |
| Implementation plan | `specs/001-litrpg-universe/plan.md` |
| Research decisions | `specs/001-litrpg-universe/research.md` |

### Key Decisions (from Clarifications)

| Decision | Answer |
|----------|--------|
| Protagonist gender | Male |
| Background | Software Engineering & Robotics |
| Dungeon structure | Standalone per novel |
| Tone | Action-comedy |
