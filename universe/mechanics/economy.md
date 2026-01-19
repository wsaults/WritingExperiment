# Economy: Currency, Commerce, and Crafting

## Currency Types

The game economy operates on multiple currency systems, each serving different purposes and operating at different scales.

### Universal Credits (UC)

**Scope**: Accepted everywhere within the game system
**Acquisition**: Enemy drops, quest rewards, item sales, achievement bonuses
**Primary Uses**: General shops, skill training, basic equipment, consumables

**Display**:
```
[Currency: 3,247 UC]
```

**Value Reference**:
| Item | Approximate Cost |
|------|------------------|
| Basic health potion | 50 UC |
| Standard weapon | 200-500 UC |
| Decent armor piece | 300-800 UC |
| Skill book (common) | 1,000-2,500 UC |
| Class change token | 50,000+ UC |

**Economy Notes**: Universal Credits are deliberately scarce in early game, moderately available mid-game, and abundant late-game. The System adjusts drop rates and shop prices to maintain this curve.

---

### Dungeon Tokens (DT)

**Scope**: Specific to individual dungeon chains
**Acquisition**: Dungeon-specific drops, objectives, hidden caches
**Primary Uses**: Dungeon shops, specialized equipment, dungeon-specific upgrades

**How They Work**: Each dungeon (or connected dungeon series) has its own token currency. Tokens from Dungeon A cannot be spent in Dungeon B's shops.

**Why This Exists**:
- Forces engagement with dungeon content rather than farming currency elsewhere
- Creates meaningful rewards for dungeon mastery
- Prevents rich contestants from buying their way through content

**Example**:
```
[Dungeon: Depths of Vellar]
[Vellar Tokens: 847]
```

**Token Conversion**: Dungeon tokens can be converted to Universal Credits at unfavorable rates (typically 10:1 or worse). This is intentionally punitive—the System wants tokens spent in dungeons.

---

### Reputation Points

**Scope**: Faction-specific
**Acquisition**: Faction quests, alignment choices, faction member kills/saves
**Primary Uses**: Faction shops, special equipment, political access

**Reputation Tiers**:
| Standing | Point Range | Benefits |
|----------|-------------|----------|
| Hostile | -1000 to -501 | Faction attacks on sight |
| Unfriendly | -500 to -1 | No shop access, limited interaction |
| Neutral | 0-499 | Basic shop access |
| Friendly | 500-1999 | Better prices, more inventory |
| Allied | 2000-4999 | Special inventory, quests |
| Exalted | 5000+ | Unique items, faction abilities |

**Major Factions** (referencing universe/bible/factions):
- Consortium Old Guard
- Horizon Syndicate
- Liberation Collective
- The Observers

Reputation with one faction may affect standing with others (allied factions gain partial rep; opposed factions may lose rep).

---

### Premium Currency: Essence

**Scope**: Universal, rare
**Acquisition**: Boss kills, achievements, dimensional anomalies, viewer tips
**Primary Uses**: Resurrection purchase, prestige items, System unlocks

**What Makes Essence Different**: Essence represents direct value to the entertainment economy. When viewers tip contestants (yes, this happens), the tip converts to Essence. High-drama moments generate Essence drops.

**Essence Costs**:
| Purchase | Cost |
|----------|------|
| Single resurrection | 500-2000 Essence |
| Legendary item | 1000+ Essence |
| Class evolution token | 750 Essence |
| System interface upgrade | 250-500 Essence |

**Economy Notes**: Essence is intentionally rare. Most contestants never accumulate more than a few hundred. Marcus's dramatic moments generate more Essence than average—viewers like him, even when he's suffering.

---

## Shops and Vendors

### Universal Shops

**Access**: Any safe zone, dungeon hub, or settlement
**Inventory**: Basic equipment, consumables, common skill books
**Pricing**: Standard rates; affected by contestant CHA

**How They Work**: Universal shops exist as System constructs—they appear when needed, stock standardized inventory, and accept Universal Credits. The shopkeepers are NPCs, but clearly artificial ones. They don't have backstories; they have *inventory*.

**Universal Shop Categories**:
- Weapons & Armor
- Consumables
- Skill Materials
- General Supplies
- Information Broker (sells hints, maps, enemy data)

---

### Dungeon Shops

**Access**: Within specific dungeon instances
**Inventory**: Dungeon-specific gear, specialized consumables, unique items
**Pricing**: Dungeon tokens; sometimes UC at premium

**Characteristics**: Dungeon shops stock items that address that dungeon's specific challenges. A fire dungeon's shop sells fire resistance gear. A puzzle dungeon's shop sells hint scrolls.

**Strategic Consideration**: Smart contestants check dungeon shops before fully committing resources. The inventory often reveals what challenges lie ahead.

---

### Faction Shops

**Access**: Faction territories, reputation-gated
**Inventory**: Faction-specific equipment, unique skills, political items
**Pricing**: Combination of UC, reputation, and faction currency

**What Makes Them Valuable**:
- Unique items unavailable elsewhere
- Equipment with faction-specific bonuses
- Skills that synergize with faction playstyles
- Access to faction-only content

**Progression**: Higher reputation unlocks better inventory tiers. The best faction items require Exalted standing.

---

### Black Markets

**Access**: Hidden locations, criminal contacts, certain dungeons
**Inventory**: Restricted items, stolen goods, faction contraband
**Pricing**: Variable; often includes non-currency costs (favors, information)

**What's Available**:
- Banned skill books
- Faction items without reputation requirements
- Resurrection tokens (at markup)
- Information about other contestants
- Exploit hints (risky—may be traps)

**Risks**:
- Scams are common
- Faction discovery damages reputation
- The System monitors black market activity
- Some "deals" are System-designed traps

---

## Item Tiers

All items have quality tiers affecting their power, durability, and value.

### Tier System

| Tier | Color | Power Level | Drop Rate | Typical Source |
|------|-------|-------------|-----------|----------------|
| Common | White/Gray | Baseline | 60% | Regular enemies, basic shops |
| Uncommon | Green | +25-50% | 25% | Elite enemies, quests |
| Rare | Blue | +75-125% | 10% | Bosses, achievements |
| Epic | Purple | +150-250% | 4% | Major bosses, faction rewards |
| Legendary | Orange | +300%+ | <1% | Unique circumstances |
| Mythic | Red | Variable | <0.01% | System grants, ascension content |

### Tier Characteristics

**Common**: Functional. Does the job. Nothing special. The bread and butter of early-game survival.

**Uncommon**: Noticeably better. Often has one bonus effect. Worth keeping but not obsessing over.

**Rare**: Significant upgrade. Usually has multiple effects or a powerful primary. Worth planning around.

**Epic**: Build-defining. These items change how you play. Worth significant investment to acquire.

**Legendary**: Game-changing. Each legendary has a unique effect that can't be replicated. Often has lore attached.

**Mythic**: Rumors, mostly. The System allegedly grants mythic items under specific circumstances. No verified drops in human contestants.

### Item Level

Within each tier, items have levels (1-100) that scale with dungeon difficulty and contestant level.

**Formula**: Item effectiveness = (Base × Tier Multiplier × Level Scaling)

A Level 50 Rare weapon substantially outperforms a Level 20 Epic weapon in raw stats, but the Epic's unique effects may still be superior.

---

## Crafting

### Crafting System Overview

Contestants can create items rather than relying solely on drops and shops. Crafting requires:
- Relevant crafting skill
- Recipe (known or discovered)
- Materials
- Crafting station (for advanced items)

### Crafting Skills

| Skill | Creates | Primary Stat |
|-------|---------|--------------|
| Blacksmithing | Weapons, armor | STR |
| Alchemy | Potions, poisons | INT |
| Cooking | Food buffs, rations | PER |
| Enchanting | Magical modifications | INT |
| Trap Making | Traps, devices | INT/AGI |
| Engineering | Constructs, mechanisms | INT |

### Material Categories

**Raw Materials**: Dropped by enemies, gathered from environment
- Monster parts (hides, bones, organs)
- Minerals (ores, gems, crystite)
- Plants (herbs, wood, fibers)
- Essences (magical extracts)

**Processed Materials**: Created from raw materials
- Ingots, cloth, treated leather
- Potions bases, enchanting dusts
- Component assemblies

**Rare Materials**: Boss drops, node spawns, achievements
- Required for Rare+ tier crafting
- Often have special properties
- Limited availability creates scarcity

### Recipe Discovery

**Methods**:
1. **Experimentation**: Combine materials, discover recipes by trial (risky—can waste materials)
2. **Purchases**: Recipes sold in shops, trainers
3. **Drops**: Recipe scrolls as loot
4. **Achievements**: Unlock recipes for specific milestones
5. **Reverse Engineering**: Analyze existing items (requires high skill)

### Crafting Quality

Crafted item quality depends on:
- Skill level
- Material quality
- Recipe complexity
- (RNG element scaled by LCK)

**Critical Crafts**: High skill + high luck can produce items above expected tier. A Rare recipe might produce an Epic result with a critical craft.

---

## Economy Balance Across Narrative

### Book 1: Scarcity

**State**: Everything is scarce. UC drops are minimal. Good equipment is rare. Every decision has opportunity cost.

**Narrative Function**: Forces difficult choices. Marcus can't buy his way out of problems. Survival requires creativity.

**Typical Currency Holdings**:
- End of Book 1: 2,000-5,000 UC
- Equipment: Mostly Common, some Uncommon
- Crafting: Basic survival items only

### Book 2: Stabilization

**State**: Resources become manageable. Steady income from cleared content. Shopping becomes meaningful rather than desperate.

**Narrative Function**: Allows investment in build development. Marcus can plan rather than just react.

**Typical Currency Holdings**:
- End of Book 2: 10,000-25,000 UC
- Equipment: Mix of Uncommon/Rare
- Crafting: Useful specialty items

### Book 3: Building

**State**: Wealth accumulates. Can afford significant upgrades. New currency sinks (faction investment, prestige items) emerge.

**Narrative Function**: Choices shift from "what can I afford" to "what should I prioritize."

**Typical Currency Holdings**:
- End of Book 3: 50,000-100,000 UC
- Equipment: Mostly Rare, some Epic
- Crafting: Meaningful contribution to build

### Book 4: Abundance (With New Sinks)

**State**: Money isn't the problem. Access and faction standing gate the valuable items. Essence becomes the true scarcity.

**Narrative Function**: Economic power doesn't solve problems. Political and personal costs dominate.

**Typical Currency Holdings**:
- End of Book 4: 200,000+ UC
- Equipment: Epic with some Legendary
- Crafting: Master-level production

### Book 5: Transcendence

**State**: Normal economy becomes irrelevant. End-game content has its own reward structures. Mythic-tier items rumored.

**Narrative Function**: Stakes are existential, not material.

**Typical Currency Holdings**:
- Currency: No longer the limiting factor
- Equipment: Legendary standard
- Crafting: Potentially Legendary creation

---

## Preventing "Too Rich" Problems

The System maintains economic tension through:

**Inflation Scaling**: Shop prices increase with contestant level
**Currency Sinks**: Revival costs, faction investments, prestige items
**New Scarcity Layers**: Essence, faction standing, unique materials
**Equipment Degradation**: Items wear out, requiring replacement
**Content Gating**: Best items require achievements, not just money
**Black Market Traps**: Easy money comes with hidden costs

---

## Marcus's Economic Philosophy

Marcus approaches economy like resource optimization:
- Calculates cost-per-value on purchases
- Invests in information over equipment
- Maintains emergency reserves
- Views currency as tool, not goal
- Exploits arbitrage opportunities when identified

His Analyst class provides economic advantages:
- Better shop deals (information leverage)
- Efficient crafting (understands material synergies)
- Identifies high-value targets (knows what's worth farming)
- Avoids scam traps (Analyze works on merchants)

---

*Word Count: ~2,000*
