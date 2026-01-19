# Stats: Primary Attributes and Derived Values

## Primary Stats Overview

The System quantifies contestant capability across seven primary attributes. Each stat starts at a baseline of 10 for adult humans, with variation based on pre-System physical and mental condition. Stats are displayed as integers from 1-999, though values above 200 are extraordinarily rare.

**Display Format**:
```
[STATS]
STR: 12  |  AGI: 14  |  END: 11
INT: 23  |  PER: 19  |  CHA: 8
LCK: 15
```

---

## Primary Stat Definitions

### Strength (STR)

**What It Affects**:
- Physical damage with melee weapons and unarmed combat
- Carrying capacity (base 10 kg + 5 kg per STR point)
- Ability to force open doors, break objects, grapple opponents
- Effectiveness of strength-based skills

**Scaling**:
| STR Range | Physical Capability |
|-----------|---------------------|
| 1-9 | Below average human |
| 10-15 | Average to athletic human |
| 16-25 | Professional athlete |
| 26-50 | Peak human, low superhuman |
| 51-100 | Clearly superhuman |
| 100+ | Can reshape local environment through force |

**How Raised**: Level-up allocation, strength-training activities, equipment bonuses, certain skills

**Soft Cap**: Returns diminish above 100 (each point provides ~70% of previous point's benefit)

---

### Agility (AGI)

**What It Affects**:
- Movement speed (base + 2% per AGI point above 10)
- Attack speed for all weapons
- Dodge chance (base 5% + 0.3% per AGI)
- Initiative in combat (who acts first)
- Effectiveness of agility-based skills (stealth, acrobatics)

**Scaling**:
| AGI Range | Physical Capability |
|-----------|---------------------|
| 1-9 | Clumsy, slow reactions |
| 10-15 | Normal human reflexes |
| 16-25 | Athletic, quick |
| 26-50 | Unnaturally fast |
| 51-100 | Bullet-timing territory |
| 100+ | Movement approaches teleportation-adjacent |

**How Raised**: Level-up allocation, agility training, equipment bonuses, certain skills

**Soft Cap**: 100 (same diminishing returns pattern)

---

### Endurance (END)

**What It Affects**:
- Health pool (primary contributor)
- Stamina pool (for physical exertion)
- Resistance to fatigue, poison, disease
- Recovery rate when resting
- Pain tolerance thresholds

**Scaling**:
| END Range | Physical Capability |
|-----------|---------------------|
| 1-9 | Fragile, tires quickly |
| 10-15 | Normal human stamina |
| 16-25 | Marathon-runner endurance |
| 26-50 | Can sustain combat for hours |
| 51-100 | Near-inexhaustible |
| 100+ | Can survive conditions that should be lethal |

**How Raised**: Level-up allocation, endurance activities, equipment, skills

**Soft Cap**: 100

---

### Intelligence (INT)

**What It Affects**:
- Mana pool (primary contributor)
- Skill effectiveness for INT-based skills
- Learning speed for new skills
- System interface clarity (higher INT = more detailed information displays)
- Problem-solving bonus to puzzle encounters

**Scaling**:
| INT Range | Mental Capability |
|-----------|-------------------|
| 1-9 | Below average cognition |
| 10-15 | Normal human intelligence |
| 16-25 | Highly intelligent |
| 26-50 | Genius-level processing |
| 51-100 | Can model complex systems intuitively |
| 100+ | Thought processes become qualitatively different |

**Special Note**: INT affects how much information the System displays. At INT 20+, contestants see additional decimal precision, subtle status effects, and more detailed skill descriptions. At INT 50+, the interface becomes nearly transparent—the System shows almost everything it's allowed to show.

**How Raised**: Level-up allocation, mental challenges, equipment, skills

**Soft Cap**: 100

---

### Perception (PER)

**What It Affects**:
- Critical hit chance (base 5% + 0.5% per PER)
- Trap detection range and accuracy
- Enemy weak point identification
- Situational awareness in combat
- Quality of Analyze skill results

**Scaling**:
| PER Range | Sensory Capability |
|-----------|-------------------|
| 1-9 | Oblivious to surroundings |
| 10-15 | Normal human awareness |
| 16-25 | Unusually observant |
| 26-50 | Notices everything in visual range |
| 51-100 | Senses extend beyond normal parameters |
| 100+ | Perceives things that shouldn't be perceptible |

**Special Note**: PER and INT synergize for analysis-type skills. A high-INT, high-PER build excels at understanding enemies and environments, even if combat stats lag behind.

**How Raised**: Level-up allocation, observation practice, equipment, skills

**Soft Cap**: 100

---

### Charisma (CHA)

**What It Affects**:
- NPC disposition and negotiation outcomes
- Party buff effectiveness when leading
- Intimidation and persuasion skill power
- Shop prices (higher CHA = better deals)
- Faction reputation gain rate

**Scaling**:
| CHA Range | Social Capability |
|-----------|-------------------|
| 1-9 | Off-putting, easily ignored |
| 10-15 | Average social presence |
| 16-25 | Naturally likeable or commanding |
| 26-50 | Magnetic personality |
| 51-100 | Can sway crowds with a word |
| 100+ | Presence affects behavior involuntarily |

**Special Note**: CHA doesn't affect other player-contestants—their actions remain under their control. It affects System-controlled entities and NPCs only.

**How Raised**: Level-up allocation, social challenges, equipment, skills

**Soft Cap**: 100

---

### Luck (LCK)

**What It Affects**:
- Loot drop quality and rarity
- Random event outcomes
- Critical hit proc rate (minor contribution)
- "Fortunate timing" frequency
- Hidden encounter chances

**Scaling**:
| LCK Range | Fortune Level |
|-----------|---------------|
| 1-9 | Actively unlucky |
| 10-15 | Normal variance |
| 16-25 | Slightly favorable outcomes |
| 26-50 | Noticeably lucky |
| 51-100 | Improbable good fortune common |
| 100+ | Reality bends toward favorable outcomes |

**Special Note**: LCK is the most mysterious stat. It doesn't guarantee outcomes—it shifts probability. High LCK won't prevent a sword through the heart, but it might mean the enemy stumbles at a crucial moment. The System seems to enjoy high-LCK contestants; they produce more dramatic reversals.

**How Raised**: Level-up allocation only. LCK cannot be trained—you're either lucky or you're not. Some equipment and skills provide bonuses.

**Soft Cap**: 100 (but LCK has the steepest diminishing returns)

---

## Derived Stats

Derived stats calculate from primary stats and level:

### Health (HP)

**Formula**: Base 100 + (END × 10) + (Level × 5)

**Example at Level 15, END 20**: 100 + 200 + 75 = 375 HP

**Display**: Red bar in interface corner; exact number visible on inspection

**Recovery**: 1% per minute at rest; faster with skills or items

---

### Mana (MP)

**Formula**: Base 50 + (INT × 8) + (Level × 3)

**Example at Level 15, INT 25**: 50 + 200 + 45 = 295 MP

**Display**: Blue bar below Health; exact number visible on inspection

**Recovery**: 2% per minute at rest; faster with skills or items

**Note**: Not all classes use Mana. Non-magical classes may have alternate resource pools (Stamina, Focus, Rage) that use different formulas.

---

### Stamina (SP)

**Formula**: Base 50 + (END × 5) + (AGI × 3)

**Example at END 20, AGI 15**: 50 + 100 + 45 = 195 SP

**Use**: Physical exertion, sprinting, heavy attacks, dodge rolls

**Recovery**: 5% per second when not exerting; pauses during combat actions

---

### Defense (DEF)

**Formula**: Base value from equipment + (END × 0.5) + skill bonuses

**Effect**: Reduces physical damage by percentage (100 DEF = ~50% reduction; diminishing returns apply)

**Display**: Numeric value in character sheet; not constantly visible

---

### Magic Resistance (MR)

**Formula**: Base value from equipment + (INT × 0.3) + (END × 0.2)

**Effect**: Reduces magical damage by percentage

**Display**: Numeric value in character sheet

---

## Marcus Chen's Starting Build

### Initial Stats (Post-System Integration)

Based on Marcus's pre-System condition—physically average, mentally sharp, emotionally guarded:

```
[MARCUS CHEN - Level 1]
STR: 11  |  AGI: 12  |  END: 10
INT: 18  |  PER: 16  |  CHA: 9
LCK: 14
```

**Stat Rationale**:
- **STR 11**: Slightly above average from handling robotics equipment
- **AGI 12**: Good reflexes from working around industrial robots
- **END 10**: Average; he forgets to exercise
- **INT 18**: Exceptional; his systems-thinking translates directly
- **PER 16**: Strong pattern recognition from debugging complex systems
- **CHA 9**: Below average; divorce fallout, emotional walls, not personable
- **LCK 14**: Slightly lucky; he's survived this long

### Allocation Strategy

Marcus prioritizes **INT** and **PER**—his natural strengths. His build philosophy: understand the system, exploit the system, survive through knowledge rather than power.

**Early Priorities (Books 1-2)**:
- INT to 25 (unlock enhanced System displays)
- PER to 20 (improve critical chance and analysis)
- END to 15 (baseline survivability)

**Mid-Game Priorities (Books 3-4)**:
- INT to 40 (mana pool for skill-heavy play)
- PER to 30 (reliable critical hits)
- AGI to 20 (mobility for survival)

**Late-Game Priorities (Book 5)**:
- Balanced growth across all stats
- INT remains highest at 60+
- No stat below 25

### Build Evolution Across Series

| Book | Level Range | Stat Focus | Narrative Reason |
|------|-------------|------------|------------------|
| 1 | 1-20 | INT/PER | Survival through understanding |
| 2 | 20-35 | INT/END | Needs durability for faction conflicts |
| 3 | 35-50 | PER/AGI | Mobility for harder dungeons |
| 4 | 50-70 | Balanced | Preparing for final challenges |
| 5 | 70-90+ | All | Ascending toward completion |

---

*Word Count: ~1,650*
