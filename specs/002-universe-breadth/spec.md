# Feature Specification: Universe Breadth Expansion

**Feature Branch**: `002-universe-breadth`
**Created**: 2026-01-19
**Status**: Draft
**Input**: User description: "review the novel universe to see if there are areas we can/should expand on breadth"

## User Scenarios & Testing *(mandatory)*

### User Story 1 - Comprehensive Species Catalog (~100 Species) (Priority: P1)

As an author writing in a universe of 12.6 million registered species, I need a comprehensive catalog of approximately 100 species at varying detail levels so that I can populate any scene—from political councils to crowded markets to dungeon encounters—with diverse, distinct beings without repetition.

**Why this priority**: The universe's scope demands species variety. A galaxy-spanning entertainment empire can't feel real with only 5 documented species. Approximately 100 species provides enough variety for any scene while remaining manageable as reference material.

**Independent Test**: Can be validated by writing 10 different scene types (council, market, dungeon, ship, settlement, etc.) each featuring 5+ distinct species with no repeats across scenes.

**Acceptance Scenarios**:

1. **Given** a scene in any galactic location, **When** populating with background characters, **Then** the author can select from 50+ visually and culturally distinct species without consulting external references.
2. **Given** the need for species variety across the 5-book series, **When** introducing new alien characters, **Then** each book can feature 10+ species not prominently featured in previous books.
3. **Given** a scene requiring specific narrative roles (merchant, warrior, scholar, trickster, etc.), **When** casting alien characters, **Then** at least 3 species options exist for each common narrative archetype.
4. **Given** D&D-inspired fantasy archetypes (psychic manipulators, hive minds, shapechangers, elemental beings, etc.), **When** needing familiar-yet-alien species, **Then** sci-fi adaptations of classic fantasy species are available.

---

### User Story 2 - Complete Founder Species Profiles (All 12) (Priority: P1)

As an author writing political intrigue involving the Consortium, I need complete profiles for all 12 founder species so that I can portray the full political landscape, historical alliances, and conflicts within the Old Guard faction.

**Why this priority**: The Founding Compact is central to galactic politics. All 12 founders must be documented to write any scene involving Consortium governance, founder rivalries, or the political machinations that affect human contestants.

**Independent Test**: Can be validated by writing a full Consortium council scene with all 12 founder representatives present, each with distinct appearance, voice, political position, and agenda.

**Acceptance Scenarios**:

1. **Given** a Consortium political scene, **When** depicting the full council, **Then** all 12 founder species have documented political positions, historical grievances, alliances, and attitudes toward humans.
2. **Given** the need to show Old Guard internal conflict, **When** selecting opposing founder species, **Then** at least 3 distinct political blocs among founders are documented with conflicting interests.
3. **Given** a scene requiring a founder ally for humans, **When** reviewing options, **Then** at least 2 founder species have documented reasons to support human advancement against Velthrani dominance.
4. **Given** the referenced "Thirteenth Founder" mystery, **When** writing hints or revelations, **Then** the 12 documented founders' histories are consistent with this mystery thread.

---

### User Story 3 - Human Survivor Culture (Priority: P2)

As an author writing Earth-side scenes and human character backstories, I need documentation of human survivor culture, factions, and settlements so that Marcus's interactions with other humans have consistent context.

**Why this priority**: Marcus interacts primarily with humans in Books 1-2. Currently, human society post-harvest exists only through character profiles (Victor, Jin, etc.) with no broader social context—settlements, human factions, survival culture, or Earth's transformed state.

**Independent Test**: Can be validated by writing a scene where Marcus arrives at a human settlement with its own rules, leaders, and culture.

**Acceptance Scenarios**:

1. **Given** a scene at a human settlement, **When** describing the location and society, **Then** at least 3 distinct human settlement types with different governance models, survival strategies, and cultures are documented.
2. **Given** the need to show human factionalism, **When** depicting political conflict, **Then** at least 3 human faction philosophies (beyond Victor's might-makes-right) are documented.
3. **Given** a scene involving Earth's transformed state, **When** describing the environment, **Then** documentation exists for how the harvest affected geography, population centers, and remaining infrastructure.

---

### User Story 4 - Additional Dungeon Themes (Priority: P2)

As an author planning Books 2-5 dungeons, I need deeper environmental variety and unique mechanics for non-Book 1 dungeons so that each book feels fresh and the "standalone dungeon per novel" principle is fully realized.

**Why this priority**: Book 1's Warehouse-7 dungeon is richly detailed (~2,100 words). Books 2-5 dungeon designs exist but with less depth, creating potential consistency issues and limiting creative options.

**Independent Test**: Can be validated by outlining a complete encounter sequence in a Book 3 dungeon with environment-specific hazards, monsters, and progression mechanics.

**Acceptance Scenarios**:

1. **Given** Book 2's underwater/bio-organic dungeon theme, **When** designing encounters, **Then** at least 5 environment-specific hazards, 5 unique monster types, and 3 dungeon-specific skills/mechanics are documented.
2. **Given** Book 4's reality-bending dungeon concept, **When** writing disorientation sequences, **Then** documentation exists for how reality manipulation manifests visually, mechanically, and psychologically.
3. **Given** the need for dungeon variety, **When** comparing all 5 book dungeons, **Then** each has at least 3 completely unique mechanics not shared with other dungeons.

---

### User Story 5 - Economy and Item System Depth (Priority: P3)

As an author writing scenes involving shops, crafting, or item acquisition, I need expanded documentation of the economic system so that loot descriptions, shop interactions, and item progressions feel consistent.

**Why this priority**: The economy.md establishes currency types and broad structure, but specific item tiers, example items, crafting recipes, and shop types are sparse. This creates friction when writing any scene involving economic activity.

**Independent Test**: Can be validated by writing a shopping scene where Marcus evaluates multiple items with clear tier differences, costs, and trade-offs.

**Acceptance Scenarios**:

1. **Given** a scene at a dungeon shop, **When** describing available items, **Then** at least 20 example items across all rarity tiers (Common to Legendary) with costs and effects are documented.
2. **Given** a crafting sequence, **When** describing the process, **Then** at least 3 crafting disciplines have documented recipes, material requirements, and output quality factors.
3. **Given** the need to show economic progression, **When** comparing Book 1 vs Book 5 item availability, **Then** clear documentation shows how item power scales across the series.

---

### User Story 6 - Galactic Geography (Priority: P3)

As an author writing scenes involving travel, galactic politics, or location-based plotting, I need documentation of galactic geography so that references to regions, systems, and travel times are consistent.

**Why this priority**: The cosmology references the "Third Spiral Confluence" and Sol System's backwater status, but no map or regional breakdown exists. This limits ability to write travel sequences or regional politics.

**Independent Test**: Can be validated by describing a character's journey from Earth to Consortium space with consistent travel time and intermediate locations.

**Acceptance Scenarios**:

1. **Given** a scene requiring galactic travel, **When** describing the route, **Then** documentation exists for major regions, travel corridors, and approximate transit times.
2. **Given** the need to show regional variation, **When** depicting different galactic areas, **Then** at least 4 named regions with distinct political affiliations, species demographics, and entertainment reputations are documented.
3. **Given** Book 5's system-level conflict, **When** describing galactic-scale stakes, **Then** documentation shows what areas would be affected and why they matter.

---

### Edge Cases

- What happens when a new species contradicts an established species' niche (duplicate ecological/narrative roles)?
- How do we handle species that were mentioned but not detailed in existing content (Keth'oran referenced in history.md)?
- What if founder species documentation reveals inconsistencies with existing political dynamics?
- How do we ensure human factions don't overshadow the galactic scope of the story?

## Requirements *(mandatory)*

### Functional Requirements

#### Species Catalog (~100 Species)

- **FR-001**: Universe MUST include approximately 100 documented species using a tiered detail system:
  - **Tier 1 (Detailed)**: 500-1,000 words - All 12 founder species + 8-10 plot-critical species (~20-22 total)
  - **Tier 2 (Standard)**: 200-400 words - Recurring species, faction-affiliated, named characters (~30-35 total)
  - **Tier 3 (Brief)**: 50-100 words - Background species, scene population, variety (~45-50 total)

- **FR-002**: All 12 founder species MUST have Tier 1 (detailed) profiles including: appearance, culture, political structure, Compact-era history, current political position, attitude toward humans, notable individuals, faction affiliations

- **FR-003**: Humans MUST be documented as a species entry including: how the galaxy perceives them, entertainment value factors, physiological traits from alien perspective, cultural observations, and galactic classification

- **FR-004**: Species catalog MUST include D&D-inspired archetypes adapted to sci-fi context:
  - Psychic manipulators (Mind Flayer inspiration)
  - Hive-mind collectives (beyond Thex)
  - Shapechangers/mimics
  - Elemental or energy-based beings
  - Scaled/reptilian variants (beyond Velthrani)
  - Insectoid species (beyond existing)
  - Aquatic/amphibious species
  - Avian species
  - Mammalian variants
  - Silicon/mineral-based life
  - Gaseous/non-corporeal entities
  - Symbiotic species pairs

- **FR-005**: Species catalog MUST include a master index organized by:
  - Alphabetical listing
  - Founder vs. non-founder status
  - Primary faction affiliation
  - Attitude toward humans (hostile/neutral/sympathetic/fascinated)
  - Narrative archetype (warrior, merchant, scholar, trickster, etc.)
  - Biology type (carbon-based, silicon, energy, etc.)

#### Human Culture

- **FR-006**: Universe MUST include documentation for at least 3 human settlement types with distinct cultures
- **FR-007**: Universe MUST include documentation for at least 3 human political/philosophical factions beyond Victor's group

#### Dungeon & Economy

- **FR-008**: Books 2-5 dungeon designs MUST be expanded to match Book 1 depth (~2,000+ words each)
- **FR-009**: Economy system MUST include at least 20 documented example items across all rarity tiers
- **FR-010**: Economy system MUST include at least 3 crafting disciplines with example recipes

#### World Structure

- **FR-011**: Universe MUST include a galactic geography document with named regions and travel context

#### Consistency

- **FR-012**: All new content MUST cross-reference existing glossary.md and use established terminology
- **FR-013**: All new content MUST align with the 7 constitution principles in `.specify/memory/constitution.md`
- **FR-014**: New species MUST NOT duplicate the narrative niche of existing species without explicit differentiation

### Key Entities

- **Species Profile (Tier 1)**: Detailed alien species documentation (500-1,000 words) for founders and plot-critical species
- **Species Profile (Tier 2)**: Standard alien species documentation (200-400 words) for recurring species
- **Species Profile (Tier 3)**: Brief alien species entry (50-100 words) for background variety
- **Species Master Index**: Categorized reference listing all ~100 species by multiple taxonomies
- **Human Species Entry**: Documentation of humans from galactic/alien perspective
- **Human Settlement**: Earth-side location with governance, culture, survival strategy
- **Human Faction**: Philosophical/political group among human survivors
- **Dungeon Environment**: Book-specific dungeon with unique theme, rules, monsters, hazards
- **Item Catalog**: Collection of equipment, consumables, and materials with tier/cost/effect data
- **Galactic Region**: Named area of space with political affiliation and travel context

## Success Criteria *(mandatory)*

### Measurable Outcomes

- **SC-001**: Author can write 10 distinct scene types each featuring 5+ unique species with zero repetition across all scenes (50+ species used)
- **SC-002**: Author can write a full Consortium council scene with all 12 founder species present, each with documented distinct appearance, voice, and political position
- **SC-003**: Author can cast any common narrative archetype (warrior, merchant, scholar, healer, trickster, diplomat, spy) with 3+ species options each
- **SC-004**: Species catalog includes representatives of all 12 D&D-inspired biological categories (psychic, hive-mind, shapechanger, elemental, reptilian, insectoid, aquatic, avian, mammalian, silicon, gaseous, symbiotic)
- **SC-005**: Humans are documented from galactic perspective with same rigor as alien species
- **SC-006**: Author can write 3 different human settlement scenes with distinct cultures and governance models
- **SC-007**: Each book's dungeon design document reaches parity with Book 1 (~2,000+ words) with unique mechanics
- **SC-008**: Author can write a shopping/crafting scene referencing at least 10 specific items with documented costs and effects
- **SC-009**: Author can describe interstellar travel with consistent geography and transit context
- **SC-010**: Species master index enables lookup by any of 6 taxonomies (alphabetical, founder status, faction, attitude, archetype, biology)

## Assumptions

- Existing species (Velthrani, Kindari, Quorathi, Thex, Vorrax) remain canonical as Tier 1 species and anchor the expanded catalog
- The 5 existing species will be classified appropriately: Velthrani as founder, others as non-founder unless retconned
- Approximately 100 species is a practical target—the universe canonically has millions, so this is representative sampling, not exhaustive
- Tier 3 (brief) species entries exist for scene population variety, not deep characterization
- D&D-inspired species are adapted to sci-fi context, not direct ports (no "space elves" in name)
- All 12 founders complete the political landscape; the "Thirteenth Founder" remains a mystery element
- Humans documented from alien perspective adds depth without changing protagonist POV
- Human factions will not become the primary focus—galactic scope remains central to the series
- Item catalog prioritizes narrative utility over completeness—example items should cover common scene needs
- Galactic geography need not be exhaustive—key regions for Books 1-5 plot points take priority

## Dependencies

- Constitution principles (`.specify/memory/constitution.md`) must be followed for all creative decisions
- Existing glossary terminology must be used consistently
- New species attitudes must align with established faction dynamics
- Human culture expansion must not contradict Marcus's backstory or existing character motivations

## Out of Scope

- Detailed languages or linguistics for alien species (beyond pronunciation guides)
- Full item database (just example items for narrative reference)
- Technical FTL travel mechanics (keep travel times narratively appropriate)
- Earth history during the harvest (keep as background, not detailed timeline)
- Detailed maps (prose descriptions sufficient)
