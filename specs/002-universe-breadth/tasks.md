# Tasks: Universe Breadth Expansion

**Input**: Design documents from `/specs/002-universe-breadth/`
**Prerequisites**: plan.md, spec.md, research.md, data-model.md, contracts/

**Tests**: Not applicable - this is creative documentation, not code. Validation is manual against success criteria.

**Organization**: Tasks are grouped by user story to enable independent creation and validation of each content area.

## Format: `[ID] [P?] [Story] Description`

- **[P]**: Can run in parallel (different files, no dependencies)
- **[Story]**: Which user story this task belongs to (e.g., US1, US2)
- All paths are relative to repository root (`universe/`)

---

## Phase 1: Setup (Directory Structure)

**Purpose**: Create directory structure and reorganize existing species files

- [ ] T001 Create species subdirectories: `universe/bible/species/founders/`, `universe/bible/species/major/`, `universe/bible/species/recurring/`, `universe/bible/species/background/`
- [ ] T002 [P] Create culture directory: `universe/culture/`
- [ ] T003 [P] Create geography directory: `universe/bible/geography/`
- [ ] T004 [P] Create items directory: `universe/mechanics/items/`
- [ ] T005 Move existing `universe/bible/species/velthrani.md` to `universe/bible/species/founders/velthrani.md`
- [ ] T006 [P] Move existing `universe/bible/species/kindari.md` to `universe/bible/species/major/kindari.md`
- [ ] T007 [P] Move existing `universe/bible/species/quorathi.md` to `universe/bible/species/major/quorathi.md`
- [ ] T008 [P] Move existing `universe/bible/species/thex-collective.md` to `universe/bible/species/major/thex-collective.md`
- [ ] T009 [P] Move existing `universe/bible/species/vorrax.md` to `universe/bible/species/major/vorrax.md`

**Checkpoint**: Directory structure ready for content creation

---

## Phase 2: Foundational (Shared Reference Files)

**Purpose**: Create index and reference files that all content will reference

**⚠️ CRITICAL**: Index structure must exist before species creation begins

- [ ] T010 Create species master index skeleton in `universe/bible/species/index.md` with 6 taxonomy sections (empty tables to be populated)
- [ ] T011 [P] Create Tier 3 species container files:
  - `universe/bible/species/background/carbon-based.md`
  - `universe/bible/species/background/silicon-based.md`
  - `universe/bible/species/background/energy-based.md`
  - `universe/bible/species/background/gaseous.md`
  - `universe/bible/species/background/symbiotic.md`

**Checkpoint**: Foundation ready - content creation can now begin

---

## Phase 3: User Story 1 - Comprehensive Species Catalog (Priority: P1) 🎯 MVP

**Goal**: Create ~100 species across three tiers providing variety for any scene type

**Independent Test**: Write 10 different scene types each featuring 5+ unique species with no repeats

### Tier 2 Species (Recurring) - 32 Species

- [ ] T012 [P] [US1] Create warrior archetype species (4): `universe/bible/species/recurring/[name].md` following Tier 2 contract
- [ ] T013 [P] [US1] Create merchant archetype species (4): `universe/bible/species/recurring/[name].md`
- [ ] T014 [P] [US1] Create scholar archetype species (3): `universe/bible/species/recurring/[name].md`
- [ ] T015 [P] [US1] Create healer archetype species (3): `universe/bible/species/recurring/[name].md`
- [ ] T016 [P] [US1] Create trickster archetype species (3): `universe/bible/species/recurring/[name].md`
- [ ] T017 [P] [US1] Create diplomat archetype species (3): `universe/bible/species/recurring/[name].md`
- [ ] T018 [P] [US1] Create spy archetype species (3): `universe/bible/species/recurring/[name].md`
- [ ] T019 [P] [US1] Create artisan archetype species (3): `universe/bible/species/recurring/[name].md`
- [ ] T020 [P] [US1] Create mystic archetype species (3): `universe/bible/species/recurring/[name].md`
- [ ] T021 [P] [US1] Create outcast archetype species (3): `universe/bible/species/recurring/[name].md`

### Tier 3 Species (Background) - 46 Species

- [ ] T022 [P] [US1] Create 15 carbon-based background species in `universe/bible/species/background/carbon-based.md`
- [ ] T023 [P] [US1] Create 10 silicon-based background species in `universe/bible/species/background/silicon-based.md`
- [ ] T024 [P] [US1] Create 8 energy-based background species in `universe/bible/species/background/energy-based.md`
- [ ] T025 [P] [US1] Create 8 gaseous/non-corporeal background species in `universe/bible/species/background/gaseous.md`
- [ ] T026 [P] [US1] Create 5 symbiotic background species in `universe/bible/species/background/symbiotic.md`

### Index Updates

- [ ] T027 [US1] Populate species master index alphabetical section in `universe/bible/species/index.md`
- [ ] T028 [US1] Populate species master index by faction affiliation in `universe/bible/species/index.md`
- [ ] T029 [US1] Populate species master index by human attitude in `universe/bible/species/index.md`
- [ ] T030 [US1] Populate species master index by narrative archetype in `universe/bible/species/index.md`
- [ ] T031 [US1] Populate species master index by biology type in `universe/bible/species/index.md`

**Checkpoint**: 78 new species documented (Tier 2 + Tier 3), index complete for them

---

## Phase 4: User Story 2 - Complete Founder Species (Priority: P1)

**Goal**: Document all 12 founder species with full Tier 1 profiles

**Independent Test**: Write a Consortium council scene with all 12 founders present, each distinct

### Founder Species Creation (11 new, 1 existing)

- [ ] T032 [P] [US2] Create founder species 2 (Velthrani Coalition bloc): `universe/bible/species/founders/[name].md` following Tier 1 contract
- [ ] T033 [P] [US2] Create founder species 3 (Velthrani Coalition bloc): `universe/bible/species/founders/[name].md`
- [ ] T034 [P] [US2] Create founder species 4 (Velthrani Coalition bloc): `universe/bible/species/founders/[name].md`
- [ ] T035 [P] [US2] Create founder species 5 (Reformist bloc): `universe/bible/species/founders/[name].md`
- [ ] T036 [P] [US2] Create founder species 6 (Reformist bloc): `universe/bible/species/founders/[name].md`
- [ ] T037 [P] [US2] Create founder species 7 (Reformist bloc - human-sympathetic): `universe/bible/species/founders/[name].md`
- [ ] T038 [P] [US2] Create founder species 8 (Isolationist bloc): `universe/bible/species/founders/[name].md`
- [ ] T039 [P] [US2] Create founder species 9 (Isolationist bloc): `universe/bible/species/founders/[name].md`
- [ ] T040 [P] [US2] Create founder species 10 (Wildcard bloc): `universe/bible/species/founders/[name].md`
- [ ] T041 [P] [US2] Create founder species 11 (Wildcard bloc - human-sympathetic): `universe/bible/species/founders/[name].md`
- [ ] T042 [P] [US2] Create founder species 12 (Wildcard bloc): `universe/bible/species/founders/[name].md`

### Existing Species Enhancement

- [ ] T043 [US2] Enhance existing `universe/bible/species/founders/velthrani.md` to include Thirteenth Founder mystery hints

### Major Non-Founder Species (Tier 1)

- [ ] T044 [P] [US2] Create humans species entry from galactic perspective: `universe/bible/species/major/humans.md`
- [ ] T045 [P] [US2] Create 1 new psychic manipulator species (D&D Mind Flayer inspired): `universe/bible/species/major/[name].md`
- [ ] T046 [P] [US2] Create 1 new shapechanger species (D&D Doppelganger inspired): `universe/bible/species/major/[name].md`
- [ ] T047 [P] [US2] Create 1 new energy being species (D&D Elemental inspired): `universe/bible/species/major/[name].md`

### Index Updates

- [ ] T048 [US2] Update species master index founder status section in `universe/bible/species/index.md`
- [ ] T049 [US2] Update all index sections with founder and major species entries

**Checkpoint**: All 12 founders documented, 4 new major species, humans documented from galactic perspective

---

## Phase 5: User Story 3 - Human Survivor Culture (Priority: P2)

**Goal**: Document human settlements, factions, and Earth's transformed state

**Independent Test**: Write a scene where Marcus arrives at a human settlement with its own rules and culture

### Human Culture Documentation

- [ ] T050 [P] [US3] Create settlement types document: `universe/culture/human-settlements.md` with 3 types (Fortress Communities, Nomadic Bands, Hidden Enclaves)
- [ ] T051 [P] [US3] Create human factions document: `universe/culture/human-factions.md` with 4 factions (Might-Makes-Right, Cooperative Survival, System Exploiters, Resistance)
- [ ] T052 [US3] Update `universe/bible/species/major/humans.md` to cross-reference culture documents

**Checkpoint**: Human survivor culture complete, 3 settlement types, 4 factions documented

---

## Phase 6: User Story 4 - Dungeon Expansions (Priority: P2)

**Goal**: Expand Books 2-5 dungeon designs to match Book 1 depth (~2,000+ words each)

**Independent Test**: Outline a complete encounter sequence in any Book 2-5 dungeon with unique mechanics

### Dungeon Design Expansions

- [ ] T053 [P] [US4] Expand Book 2 dungeon design: `universe/plot/book-2/dungeon-design.md` to ~2,000 words (underwater/bio-organic theme)
- [ ] T054 [P] [US4] Expand Book 3 dungeon design: `universe/plot/book-3/dungeon-design.md` to ~2,000 words (social/political theme)
- [ ] T055 [P] [US4] Expand Book 4 dungeon design: `universe/plot/book-4/dungeon-design.md` to ~2,000 words (reality-bending theme)
- [ ] T056 [P] [US4] Expand Book 5 dungeon design: `universe/plot/book-5/dungeon-design.md` to ~2,000 words (system-level theme)

### Dungeon Consistency Check

- [ ] T057 [US4] Verify each dungeon has 3+ unique mechanics not shared with others, document in each file

**Checkpoint**: All 5 dungeons at parity (~2,000+ words each), unique mechanics per dungeon

---

## Phase 7: User Story 5 - Economy & Items (Priority: P3)

**Goal**: Create item catalog with 20+ example items and crafting documentation

**Independent Test**: Write a shopping scene referencing 10+ items with costs and effects

### Item Documentation

- [ ] T058 [US5] Create item catalog: `universe/mechanics/items/item-catalog.md` with 20+ items across all tiers
  - 5+ weapons (Common to Legendary)
  - 4+ armor/defense items
  - 6+ consumables
  - 3+ tools/utility
  - 2+ skill enhancements
- [ ] T059 [US5] Update `universe/mechanics/economy.md` with crafting disciplines (3 disciplines with recipes)

**Checkpoint**: Item catalog complete, crafting documented, economy enhanced

---

## Phase 8: User Story 6 - Galactic Geography (Priority: P3)

**Goal**: Document galactic regions and travel context

**Independent Test**: Describe a journey from Earth to Consortium space with consistent geography

### Geography Documentation

- [ ] T060 [US6] Create galactic geography document: `universe/bible/geography/galactic-regions.md` with 4 regions (Core Worlds, Third Spiral Confluence, Outer Rim, Quarantine Zones)
- [ ] T061 [US6] Update `universe/bible/cosmology.md` to cross-reference geography document

**Checkpoint**: Galactic geography complete, travel context established

---

## Phase 9: Polish & Cross-Cutting Concerns

**Purpose**: Final validation, glossary updates, consistency checks

- [ ] T062 Update `universe/bible/glossary.md` with all new species names (alphabetical)
- [ ] T063 Update `universe/bible/glossary.md` with new terms (settlement types, faction names, region names, key items)
- [ ] T064 Constitution compliance check: Verify all content against 7 principles in `.specify/memory/constitution.md`
- [ ] T065 Cross-reference validation: Verify all faction references match `universe/bible/factions/`
- [ ] T066 Run quickstart.md validation scenarios (10 scene types with 5+ species each)
- [ ] T067 Final species count verification: Confirm ~100 species documented across all tiers

---

## Dependencies & Execution Order

### Phase Dependencies

- **Setup (Phase 1)**: No dependencies - can start immediately
- **Foundational (Phase 2)**: Depends on Setup - BLOCKS content creation
- **US1 Species Catalog (Phase 3)**: Depends on Foundational
- **US2 Founders (Phase 4)**: Depends on Foundational - can run parallel with US1
- **US3 Human Culture (Phase 5)**: Depends on Foundational - can run parallel with US1/US2
- **US4 Dungeons (Phase 6)**: Depends on Foundational - can run parallel with US1-3
- **US5 Economy (Phase 7)**: Depends on Foundational - can run parallel with US1-4
- **US6 Geography (Phase 8)**: Depends on Foundational - can run parallel with US1-5
- **Polish (Phase 9)**: Depends on ALL user stories complete

### User Story Independence

All user stories (US1-US6) can proceed in parallel after Foundational phase:

| Story | Content Area | Parallel Safe? |
|-------|--------------|----------------|
| US1 | Species Catalog (Tier 2/3) | Yes |
| US2 | Founders + Major Species | Yes |
| US3 | Human Culture | Yes |
| US4 | Dungeon Expansions | Yes |
| US5 | Economy & Items | Yes |
| US6 | Galactic Geography | Yes |

### Within Each User Story

- Files marked [P] can be created in parallel
- Index updates should follow content creation
- Cross-reference updates are final steps

---

## Parallel Opportunities

### Maximum Parallelism (Phase 3-8)

After Foundational phase, ALL of these can run simultaneously:

```text
US1: T012-T031 (20 tasks) - Species Tier 2/3 creation
US2: T032-T049 (18 tasks) - Founders and major species
US3: T050-T052 (3 tasks) - Human culture
US4: T053-T057 (5 tasks) - Dungeon expansions
US5: T058-T059 (2 tasks) - Economy & items
US6: T060-T061 (2 tasks) - Geography
```

### Within US1 (Species Catalog)

```text
# All archetype species can be created in parallel:
T012-T021 (10 parallel tasks for Tier 2 archetypes)

# All biology-grouped files can be created in parallel:
T022-T026 (5 parallel tasks for Tier 3 species)
```

### Within US2 (Founders)

```text
# All 11 new founder species can be created in parallel:
T032-T042 (11 parallel tasks)

# All 4 major species can be created in parallel:
T044-T047 (4 parallel tasks)
```

---

## Implementation Strategy

### MVP First (US1 + US2 Only)

1. Complete Phase 1: Setup
2. Complete Phase 2: Foundational
3. Complete Phase 3: US1 (Species Catalog)
4. Complete Phase 4: US2 (Founders)
5. **STOP and VALIDATE**: Test by writing multi-species scene
6. Deliver MVP with ~100 species

### Incremental Delivery

1. Setup + Foundational → Structure ready
2. Add US1 + US2 → Species complete (MVP!)
3. Add US3 → Human culture complete
4. Add US4 → Dungeons complete
5. Add US5 → Economy complete
6. Add US6 → Geography complete
7. Polish → Full feature complete

### Single Author Strategy

Sequential priority order:
1. Phase 1-2 (Setup/Foundation)
2. US1 (Species Tier 2/3) - highest volume
3. US2 (Founders) - most critical for plot
4. US3-6 in priority order
5. Phase 9 (Polish)

---

## Task Summary

| Phase | User Story | Task Count | Parallelizable |
|-------|------------|------------|----------------|
| 1 | Setup | 9 | 4 |
| 2 | Foundational | 2 | 1 |
| 3 | US1 - Species Catalog | 20 | 15 |
| 4 | US2 - Founders | 18 | 15 |
| 5 | US3 - Human Culture | 3 | 2 |
| 6 | US4 - Dungeons | 5 | 4 |
| 7 | US5 - Economy | 2 | 0 |
| 8 | US6 - Geography | 2 | 1 |
| 9 | Polish | 6 | 0 |
| **Total** | | **67** | **42** |

---

## Notes

- [P] tasks = different files, no dependencies
- [US#] label maps task to specific user story
- Each user story is independently completable and testable
- Species creation tasks include naming - use guidelines from research.md
- Tier contracts in `specs/002-universe-breadth/contracts/` define required fields
- Constitution compliance required for all content
- Commit after each logical group of related species
