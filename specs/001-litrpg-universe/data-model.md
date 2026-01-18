# Data Model: LitRPG Universe Bible Structure

**Branch**: `001-litrpg-universe` | **Date**: 2026-01-17
**Purpose**: Define the structural schema for all universe documentation

---

## Entity Relationship Overview

```
┌─────────────────────────────────────────────────────────────────┐
│                         THE UNIVERSE                            │
├─────────────────────────────────────────────────────────────────┤
│  ┌──────────┐    governs    ┌──────────┐    contains           │
│  │  System  │──────────────▶│  Games   │──────────────┐        │
│  └──────────┘               └──────────┘              │        │
│       │                          │                    ▼        │
│       │ interfaces               │ occur in    ┌──────────┐   │
│       ▼                          ▼              │ Dungeons │   │
│  ┌──────────┐              ┌──────────┐        └──────────┘   │
│  │ Players  │◀─────────────│ Factions │              │        │
│  └──────────┘   sponsor    └──────────┘              │        │
│       │                          │                    │        │
│       │ include                  │ employ            │ spawn   │
│       ▼                          ▼                    ▼        │
│  ┌──────────┐              ┌──────────┐        ┌──────────┐   │
│  │Characters│              │  Aliens  │        │ Monsters │   │
│  └──────────┘              └──────────┘        └──────────┘   │
└─────────────────────────────────────────────────────────────────┘
```

---

## Core Entities

### 1. The System

**Definition**: Omnipresent AI/force that governs all game mechanics

**Attributes**:
| Field | Type | Description |
|-------|------|-------------|
| name | string | What contestants call it (may vary by culture) |
| interface_style | enum | How it communicates (text boxes, voice, etc.) |
| personality | text | Sardonic, neutral, helpful—affects tone |
| origin | text | Where it came from (mystery to be revealed) |
| limitations | list | What it cannot or will not do |
| hidden_agenda | text | Series-level mystery about its true purpose |

**Relationships**:
- Governs: Games (1:many)
- Interfaces with: Players (1:many)
- Created by: Unknown (series mystery)

**Validation Rules**:
- Personality must be consistent across appearances
- Limitations established in Book 1 cannot be contradicted later
- Hidden agenda must have planted clues by Book 3

---

### 2. Games

**Definition**: Individual survival competitions within the universe

**Attributes**:
| Field | Type | Description |
|-------|------|-------------|
| name | string | Official game designation |
| dungeon_id | ref | Which dungeon hosts this game |
| contestant_count | int | Starting population |
| rules | list | Game-specific constraints |
| rewards | list | What survivors can win |
| audience_rating | metric | Popularity affects resources |

**Relationships**:
- Hosted in: Dungeon (many:1)
- Governed by: System (many:1)
- Watched by: Audience (many:many)
- Funded by: Factions (many:many)

---

### 3. Dungeons

**Definition**: Standalone challenge environments (one primary per novel)

**Attributes**:
| Field | Type | Description |
|-------|------|-------------|
| name | string | Dungeon designation |
| theme | string | Environmental/aesthetic concept |
| unique_rules | list | Mechanics specific to this dungeon |
| difficulty_tier | int | Relative to series progression |
| monster_types | list | Creature categories present |
| environmental_hazards | list | Non-monster threats |
| loot_tables | object | Reward distribution rules |
| boss_encounter | ref | Final challenge design |

**Validation Rules**:
- Each dungeon must have at least 3 unique rules
- Theme must be distinct from previous dungeons
- Difficulty tier must equal or exceed previous

**Examples** (5 novels):
1. Book 1: Industrial/mechanical theme (protagonist's comfort zone subverted)
2. Book 2: Organic/biological horror theme (force adaptation)
3. Book 3: Social/political dungeon (faction intrigue focus)
4. Book 4: Abstract/reality-bending theme (high concept)
5. Book 5: System-level challenge (confrontation with game itself)

---

### 4. Factions

**Definition**: Major alien power structures competing for influence

**Attributes**:
| Field | Type | Description |
|-------|------|-------------|
| name | string | Faction designation |
| philosophy | text | Core belief about contestant treatment |
| economic_interests | list | What they gain from games |
| political_stance | enum | Reformist, traditionalist, abolitionist, etc. |
| key_members | list | Named representatives |
| relationship_to_protagonist | text | How they view/interact with MC |

**Minimum Count**: 4 factions required

**Required Philosophies** (must cover spectrum):
- [ ] One faction that views contestants as resources
- [ ] One faction that views contestants with sympathy
- [ ] One faction focused purely on profit/ratings
- [ ] One faction with hidden/complex agenda

---

### 5. Species (Alien Races)

**Definition**: Distinct alien civilizations in the universe

**Attributes**:
| Field | Type | Description |
|-------|------|-------------|
| name | string | Species designation |
| physiology | text | Physical characteristics |
| culture | text | Values, customs, society structure |
| lifespan | string | Relative to humans |
| attitude_to_humans | enum | Hostile, sympathetic, indifferent, fascinated |
| faction_affiliations | list | Which factions they dominate/support |
| notable_individuals | list | Named characters of this species |

**Minimum Count**: 5 species required

**Required Coverage**:
- [ ] At least one species hostile to humans
- [ ] At least one species sympathetic to humans
- [ ] At least one species indifferent/transactional
- [ ] At least one species that finds humans fascinating

---

### 6. Characters

**Definition**: Named individuals with roles in the narrative

**Subtypes**:

#### 6a. Protagonist

**Attributes**:
| Field | Type | Description |
|-------|------|-------------|
| name | string | Full name |
| age | int | At series start |
| background | text | Pre-apocalypse life |
| skills | list | Non-game competencies |
| personality_traits | list | Core characteristics |
| voice_samples | list | Example internal monologue |
| moral_line | text | What they won't do |
| character_arc | text | How they change across series |
| relationships | list | Pre-existing and developing |

#### 6b. Companions

**Attributes**:
| Field | Type | Description |
|-------|------|-------------|
| name | string | Designation |
| species | ref | Human or alien |
| role | enum | Combat, support, comic relief, etc. |
| relationship_to_protagonist | text | How they connect |
| independent_goals | list | What they want beyond protagonist |
| arc | text | Their own development |
| fate | enum | Survives, dies, departs, unknown |

**Validation Rules**:
- At least one non-human companion required
- Each companion must have independent goals
- At least one must face significant loss/departure

#### 6c. Antagonists

**Attributes**:
| Field | Type | Description |
|-------|------|-------------|
| name | string | Designation |
| threat_level | enum | Personal, faction, system-level |
| motivation | text | Why they oppose protagonist |
| methods | list | How they create conflict |
| redeemability | enum | None, possible, likely |

---

### 7. Game Mechanics

**Definition**: The LitRPG system rules

#### 7a. Stats

**Required Stats**:
| Stat | Description | Protagonist Starting Range |
|------|-------------|---------------------------|
| Strength | Physical power | Below average (not physical type) |
| Agility | Speed/reflexes | Average |
| Endurance | Stamina/health | Average |
| Intelligence | Mental processing | Above average (SWE background) |
| Perception | Awareness/detection | Above average (pattern recognition) |
| Charisma | Social influence | Below average (introvert engineer) |
| Luck | Random factor | Variable (plot device) |

#### 7b. Classes

**Design Principle**: Classes are templates, not prisons. Protagonist should subvert/exploit class expectations.

**Protagonist Class**: To be determined—should play against type (e.g., gets "support" class, uses it offensively)

#### 7c. Skills

**Skill Categories**:
- Combat skills
- Utility skills
- Social skills
- Crafting skills
- Dungeon-specific skills (unlock per environment)

**Progression**: Skills level through use, not point allocation (more organic)

#### 7d. Economy

**Currency Types**:
- Universal currency (works everywhere)
- Dungeon-specific currency (local only)
- Reputation/favor (non-monetary)

**Economic Sinks**:
- Equipment
- Consumables
- Information
- Services (healing, crafting, etc.)
- Bribes/favors

---

## State Transitions

### Protagonist Power Progression

```
Book 1: Survival Mode
  └─▶ Discovers system basics
  └─▶ Finds initial build direction
  └─▶ Reaches competent (not dominant)

Book 2: Exploitation Mode
  └─▶ Actively games the system
  └─▶ Attracts faction attention
  └─▶ Reaches locally powerful

Book 3: Political Mode
  └─▶ Navigates faction conflicts
  └─▶ Gains allies and enemies
  └─▶ Reaches influential

Book 4: Reality-Bending Mode
  └─▶ Pushes system limits
  └─▶ Discovers deeper truths
  └─▶ Reaches exceptional

Book 5: Confrontation Mode
  └─▶ Challenges system itself
  └─▶ Series climax
  └─▶ Resolution
```

### Faction Relationship States

```
Unknown ──▶ Aware ──▶ Interested ──▶ Allied/Hostile
                                         │
                                         ▼
                                   Betrayed/Converted
```

---

## Consistency Rules

### Cross-Book Validation

- [ ] Stats established in Book 1 use same scale throughout
- [ ] Skills introduced must remain available (can't disappear)
- [ ] Currency values maintain consistent purchasing power
- [ ] Character voices don't drift between books
- [ ] Faction philosophies remain recognizable
- [ ] System rules don't contradict earlier statements

### Mystery Budget

| Mystery | Planted By | Revealed By | Status |
|---------|------------|-------------|--------|
| System origin | Book 1 | Book 4-5 | Required |
| Why Earth selected | Book 1 | Book 3 | Required |
| Protagonist's hidden potential | Book 1 | Book 2 | Required |
| True faction motives | Books 1-2 | Books 3-4 | Required |
| Endgame stakes | Books 2-3 | Book 5 | Required |
