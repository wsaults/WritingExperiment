# Game Mechanics Rules

**Applies to**: `universe/mechanics/**/*.md`

## System Rules Requirements (`system-rules.md`)

### Core System Documentation

**System Manifestation**:
- How contestants perceive the interface
- Visual characteristics (colors, fonts, positioning)
- Notification categories and styles
- Audio components

**System Personality**:
- Communication patterns (formal, commentary, cryptic)
- What System reveals/hides
- System biases (rewarded vs punished behaviors)

**What System Can/Cannot Do**:
- Constraints on System power
- Policy limitations vs physics limitations

Word count: 1,500-2,500 words

## Stats Requirements (`stats.md`)

### Primary Stats

For each stat, document:
- Name and abbreviation
- What it affects
- How it's raised
- Soft/hard caps
- Display format

**Required Stats**:
| Stat | Abbr | Primary Effect |
|------|------|----------------|
| Strength | STR | Physical damage, carry weight |
| Agility | AGI | Speed, dodge, attack speed |
| Endurance | END | Health pool, stamina |
| Intelligence | INT | Skill effectiveness, mana |
| Perception | PER | Detection, crit chance |
| Charisma | CHA | NPC interaction, party buffs |
| Luck | LCK | Drop rates, random events |

### Derived Stats
- Health (from END + level)
- Mana/Energy (from INT + class)
- Defense (from equipment + stats)

### Protagonist Build
- Initial stat distribution
- Stat priorities
- Evolution across series

Word count: 1,000-2,000 words

## Classes Requirements (`classes.md`)

Document:
- How classes are assigned/chosen
- Class tiers (basic → advanced → prestige)
- Multi-classing rules
- Class change mechanics
- Protagonist's class and evolution path
- Minimum 10 example classes with roles and abilities

Word count: 1,500-2,500 words

## Skills Requirements (`skills.md`)

### Skill Categories
- Combat skills
- Utility skills
- Social skills
- Crafting skills
- Passive skills
- Dungeon-specific skills

### Document
- How skills are learned
- How skills level up
- Skill ranks/tiers
- Skill synergies
- Protagonist's key skills with evolution
- Skill display format

Word count: 2,000-3,500 words

## Economy Requirements (`economy.md`)

### Currency Types
| Currency | Scope | Acquisition | Uses |
|----------|-------|-------------|------|
| Universal | Everywhere | Drops, rewards | General shops |
| Dungeon-specific | One dungeon | Local drops | Local shops |
| Reputation | Faction-specific | Actions | Faction rewards |

### Document
- Shops & vendors
- Item tiers (Common → Legendary)
- Crafting system
- Economy balance across series

Word count: 1,500-2,500 words

## Consistency Validation

### Cross-Reference Checklist
- [ ] Stats referenced in skills match stats.md
- [ ] Class abilities use consistent terminology
- [ ] Economy values are proportional
- [ ] Skill costs match economy expectations
- [ ] Level requirements are consistent

### Protagonist Build Tracker

| Book | Level Range | Key Stats | Key Skills | Key Items |
|------|-------------|-----------|------------|-----------|
| 1 | 1-20 | INT/PER | [defined] | [defined] |
| 2 | 20-40 | [defined] | [defined] | [defined] |
| 3 | 40-60 | [defined] | [defined] | [defined] |
| 4 | 60-80 | [defined] | [defined] | [defined] |
| 5 | 80-100+ | [defined] | [defined] | [defined] |

## Constitution Alignment

- Principle V (Mechanics Integrity) - primary validation
- No deus ex machina power-ups without setup and cost
- Readers who care about builds can theorize; readers who don't can skim safely
