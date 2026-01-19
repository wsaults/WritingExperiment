# Tasks: Multi-Novel LitRPG Universe

**Input**: Design documents from `/specs/001-litrpg-universe/`
**Prerequisites**: plan.md (required), spec.md (required), research.md, data-model.md, contracts/

**Tests**: Not applicable—this is a creative writing project, not software. Validation is via contract checklists.

**Organization**: Tasks are grouped by user story to enable independent implementation and validation of each story's deliverables.

## Format: `[ID] [P?] [Story?] Description`

- **[P]**: Can run in parallel (different files, no dependencies)
- **[Story]**: Which user story this task belongs to (e.g., US1, US2, US3, US4)
- Include exact file paths in descriptions

## Path Conventions

```text
universe/
├── bible/           # Universe Bible (US1)
├── characters/      # Character Bible (US4)
├── mechanics/       # Game Mechanics (US3)
├── plot/            # Plot Outlines (US2)
└── style/           # Writing Style (US1)
```

---

## Phase 1: Setup (Project Structure)

**Purpose**: Create directory structure and foundational files

- [ ] T001 Create directory structure per plan.md in universe/
- [ ] T002 [P] Create universe/bible/ directory with placeholder files
- [ ] T003 [P] Create universe/characters/ directory with placeholder files
- [ ] T004 [P] Create universe/mechanics/ directory with placeholder files
- [ ] T005 [P] Create universe/plot/ directory with book-1/ through book-5/ subdirectories
- [ ] T006 [P] Create universe/style/ directory with placeholder files
- [ ] T007 Copy glossary template to universe/bible/glossary.md

**Checkpoint**: Directory structure ready for content creation

---

## Phase 2: Foundational (Shared Infrastructure)

**Purpose**: Core world-building that ALL user stories depend on

**⚠️ CRITICAL**: No user story work can begin until this phase is complete

- [ ] T008 Create universe/bible/cosmology.md with core universe rules per contracts/universe-bible.md
- [ ] T009 Define The System entity in universe/bible/cosmology.md (personality, interface, limitations)
- [ ] T010 Establish game show premise and economics in universe/bible/cosmology.md
- [ ] T011 Create universe/bible/glossary.md with initial canonical terminology

**Checkpoint**: Foundation ready - universe rules established, user story work can begin

---

## Phase 3: User Story 1 - Reader Discovers Universe (Priority: P1) 🎯 MVP

**Goal**: Create all world-building needed for a reader to immediately understand and engage with the universe in Book 1

**Independent Test**: Beta reader can complete first 3 chapters and accurately describe universe rules, tone, and protagonist situation

### Universe Bible (US1)

- [ ] T012 [P] [US1] Create universe/bible/species/species-hostile.md (hostile alien species)
- [ ] T013 [P] [US1] Create universe/bible/species/species-sympathetic.md (sympathetic alien species)
- [ ] T014 [P] [US1] Create universe/bible/species/species-indifferent.md (transactional alien species)
- [ ] T015 [P] [US1] Create universe/bible/species/species-fascinated.md (fascinated by humans species)
- [ ] T016 [P] [US1] Create universe/bible/species/species-wildcard.md (5th required species)
- [ ] T017 [P] [US1] Create universe/bible/factions/faction-resource.md (views contestants as resources)
- [ ] T018 [P] [US1] Create universe/bible/factions/faction-sympathetic.md (sympathetic to contestants)
- [ ] T019 [P] [US1] Create universe/bible/factions/faction-profit.md (profit/ratings focused)
- [ ] T020 [P] [US1] Create universe/bible/factions/faction-hidden.md (hidden agenda faction)
- [ ] T101 [US1] Add faction representative profiles to each faction file (named NPCs who interact directly with contestants per FR-011)
- [ ] T021 [US1] Create universe/bible/history.md with game origins and Earth selection
- [ ] T022 [US1] Update universe/bible/glossary.md with all species and faction terms

### Style Guide (US1)

- [ ] T023 [P] [US1] Create universe/style/tone-guide.md with action-comedy guidelines per contracts/style-guide.md
- [ ] T024 [P] [US1] Create universe/style/prose-examples.md with action scene templates
- [ ] T025 [US1] Add dialogue scene templates to universe/style/prose-examples.md
- [ ] T026 [US1] Add exposition delivery templates to universe/style/prose-examples.md
- [ ] T027 [US1] Define System interface format in universe/style/prose-examples.md

**Checkpoint**: Reader Discovers Universe complete - world-building sufficient for Book 1 opening

---

## Phase 4: User Story 4 - Reader Connects With Characters (Priority: P1)

**Goal**: Create character bibles that enable readers to form emotional bonds with protagonist and key cast

**Independent Test**: Beta reader can articulate what makes protagonist entertaining and worth rooting for after 5 chapters

### Protagonist (US4)

- [ ] T028 [US4] Create universe/characters/protagonist.md with identity section per contracts/character-bible.md
- [ ] T029 [US4] Add background section to universe/characters/protagonist.md (SWE/Robotics details, divorce, startup)
- [ ] T030 [US4] Add personality section to universe/characters/protagonist.md (traits, flaws, moral line)
- [ ] T031 [US4] Add voice section with 15+ sample passages to universe/characters/protagonist.md
- [ ] T032 [US4] Add character arc section to universe/characters/protagonist.md (Books 1-5 evolution)

### Voice Guide (US4)

- [ ] T033 [US4] Create universe/style/voice-guide.md with combat situation samples
- [ ] T034 [US4] Add discovery/exploration samples to universe/style/voice-guide.md
- [ ] T035 [US4] Add social interaction samples to universe/style/voice-guide.md
- [ ] T036 [US4] Add low moment samples to universe/style/voice-guide.md
- [ ] T037 [US4] Add victory/success samples to universe/style/voice-guide.md

### Supporting Cast (US4)

- [ ] T038 [P] [US4] Create universe/characters/companions/companion-nonhuman.md (primary non-human companion)
- [ ] T039 [P] [US4] Create universe/characters/companions/companion-human.md (human ally with potential betrayal/departure)
- [ ] T040 [P] [US4] Create universe/characters/companions/companion-complex.md (enemy-turned-friend or vice versa)
- [ ] T041 [P] [US4] Create universe/characters/antagonists/antagonist-personal.md (early books threat)
- [ ] T042 [P] [US4] Create universe/characters/antagonists/antagonist-faction.md (mid books threat)
- [ ] T043 [P] [US4] Create universe/characters/antagonists/antagonist-system.md (late books threat)
- [ ] T044 [US4] Create universe/characters/supporting/ files for 5+ recurring characters
- [ ] T045 [US4] Validate voice differentiation across all major characters

**Checkpoint**: Reader Connects With Characters complete - protagonist and cast fully defined

---

## Phase 5: User Story 3 - Reader Engages With Game Mechanics (Priority: P2)

**Goal**: Create complete LitRPG system that readers can track, theorize about, and debate

**Independent Test**: Mechanically-minded reader can reconstruct protagonist's build from memory after reading a novel

### Core Mechanics (US3)

- [ ] T046 [US3] Create universe/mechanics/system-rules.md with core System principles per contracts/mechanics-system.md
- [ ] T047 [US3] Add leveling mechanics to universe/mechanics/system-rules.md
- [ ] T048 [US3] Add death/respawn rules to universe/mechanics/system-rules.md
- [ ] T049 [US3] Create universe/mechanics/stats.md with all 7 primary stats defined
- [ ] T050 [US3] Add derived stats to universe/mechanics/stats.md
- [ ] T051 [US3] Define protagonist starting build in universe/mechanics/stats.md

### Classes & Skills (US3)

- [ ] T052 [US3] Create universe/mechanics/classes.md with class system overview
- [ ] T053 [US3] Define protagonist's class and subversion strategy in universe/mechanics/classes.md
- [ ] T054 [US3] Add 10+ example classes to universe/mechanics/classes.md
- [ ] T055 [US3] Create universe/mechanics/skills.md with skill categories
- [ ] T056 [US3] Add skill progression rules to universe/mechanics/skills.md
- [ ] T057 [US3] Define protagonist's key skills in universe/mechanics/skills.md

### Economy (US3)

- [ ] T058 [US3] Create universe/mechanics/economy.md with currency types
- [ ] T059 [US3] Add shops and vendors to universe/mechanics/economy.md
- [ ] T060 [US3] Add item tiers to universe/mechanics/economy.md
- [ ] T061 [US3] Add crafting system to universe/mechanics/economy.md
- [ ] T062 [US3] Define economy balance across series in universe/mechanics/economy.md

### Consistency Validation (US3)

- [ ] T063 [US3] Create protagonist build tracker table (levels, stats, skills per book)
- [ ] T064 [US3] Cross-reference all mechanics documents for consistency
- [ ] T065 [US3] Update universe/bible/glossary.md with all mechanics terms

**Checkpoint**: Reader Engages With Mechanics complete - full LitRPG system defined and consistent

---

## Phase 6: User Story 2 - Reader Follows Multi-Novel Arc (Priority: P2)

**Goal**: Create plot outlines that ensure each book satisfies while demanding sequels, with mysteries that pay off

**Independent Test**: Reader finishes Book 1 and reports wanting to read Book 2 (85%+ target)

### Series Arc (US2)

- [ ] T066 [US2] Create universe/plot/series-arc.md with meta-plot overview per contracts/plot-outline.md
- [ ] T067 [US2] Define stakes escalation across 5 books in universe/plot/series-arc.md
- [ ] T068 [US2] Create mystery thread tracking table in universe/plot/series-arc.md
- [ ] T102 [US2] Document manipulation opportunities in universe/plot/series-arc.md (where protagonist can play factions against each other per FR-013)
- [ ] T069 [US2] Define character arc summaries in universe/plot/series-arc.md
- [ ] T103 [US2] Define significant loss/departure events in universe/plot/series-arc.md (which companion dies/departs, which book, per FR-022)

### Book 1 Outline (US2)

- [ ] T070 [US2] Create universe/plot/book-1/outline.md with 3-act structure
- [ ] T071 [US2] Create universe/plot/book-1/dungeon-design.md (Industrial/mechanical theme)
- [ ] T104 [US2] Add monster ecology section to all dungeon-design.md files (creature origins, respawn logic per FR-007)
- [ ] T072 [US2] Create universe/plot/book-1/character-introductions.md
- [ ] T073 [US2] Define Book 1 cliffhanger and series hook in universe/plot/book-1/outline.md

### Book 2 Outline (US2)

- [ ] T074 [P] [US2] Create universe/plot/book-2/outline.md with 3-act structure
- [ ] T075 [P] [US2] Create universe/plot/book-2/dungeon-design.md (Organic/biological theme)
- [ ] T076 [US2] Define faction involvement escalation in universe/plot/book-2/outline.md

### Book 3 Outline (US2)

- [ ] T077 [P] [US2] Create universe/plot/book-3/outline.md with 3-act structure
- [ ] T078 [P] [US2] Create universe/plot/book-3/dungeon-design.md (Social/political theme)
- [ ] T079 [US2] Define Earth selection revelation in universe/plot/book-3/outline.md

### Book 4 Outline (US2)

- [ ] T080 [P] [US2] Create universe/plot/book-4/outline.md with 3-act structure
- [ ] T081 [P] [US2] Create universe/plot/book-4/dungeon-design.md (Abstract/reality-bending theme)
- [ ] T082 [US2] Define System secrets reveal in universe/plot/book-4/outline.md

### Book 5 Outline (US2)

- [ ] T083 [P] [US2] Create universe/plot/book-5/outline.md with 3-act structure
- [ ] T084 [P] [US2] Create universe/plot/book-5/dungeon-design.md (System-level challenge)
- [ ] T085 [US2] Define series resolution and all mystery payoffs in universe/plot/book-5/outline.md

### Arc Validation (US2)

- [ ] T086 [US2] Verify all mysteries in series-arc.md have plant/hint/reveal defined
- [ ] T087 [US2] Verify stakes escalation is clear across all 5 book outlines
- [ ] T088 [US2] Verify each book has standalone satisfaction + series hook
- [ ] T105 [US2] Validate pacing balance in each book outline (70% action/plot, 20% comedy, 10% character beats per FR-029)

**Checkpoint**: Reader Follows Multi-Novel Arc complete - 5-book series fully outlined

---

## Phase 7: Polish & Cross-Cutting Concerns

**Purpose**: Final validation and consistency checks across all deliverables

- [ ] T089 Run full contract validation against contracts/universe-bible.md
- [ ] T090 Run full contract validation against contracts/character-bible.md
- [ ] T091 Run full contract validation against contracts/mechanics-system.md
- [ ] T092 Run full contract validation against contracts/plot-outline.md
- [ ] T093 Run full contract validation against contracts/style-guide.md
- [ ] T094 [P] Final glossary update in universe/bible/glossary.md
- [ ] T095 [P] Constitution compliance check against all 7 principles
- [ ] T096 Cross-reference check: mechanics mentioned in plot match mechanics docs
- [ ] T097 Cross-reference check: characters in plot match character docs
- [ ] T098 Cross-reference check: all faction/species references consistent
- [ ] T099 Run quickstart.md validation process
- [ ] T100 Update spec.md status from Draft to Complete

---

## Dependencies & Execution Order

### Phase Dependencies

- **Setup (Phase 1)**: No dependencies - can start immediately
- **Foundational (Phase 2)**: Depends on Setup - BLOCKS all user stories
- **US1 & US4 (Phase 3-4)**: Both P1, can run in parallel after Foundational
- **US2 & US3 (Phase 5-6)**: Both P2, can run in parallel after P1 stories complete
- **Polish (Phase 7)**: Depends on all user stories being complete

### User Story Dependencies

- **US1 (Reader Discovers Universe)**: Can start after Foundational
- **US4 (Reader Connects With Characters)**: Can start after Foundational, benefits from US1 world context
- **US3 (Reader Engages With Mechanics)**: Can start after Foundational, should reference US1 world
- **US2 (Reader Follows Multi-Novel Arc)**: Benefits from US1 (world), US3 (mechanics), US4 (characters)

### Parallel Opportunities

Within each user story phase, tasks marked [P] can run in parallel:

- Phase 1: T002-T006 (directory creation)
- Phase 3 (US1): T012-T020 (species + factions), T023-T024 (style docs)
- Phase 4 (US4): T038-T043 (companions + antagonists)
- Phase 6 (US2): T074-T084 (book outlines 2-5)

---

## Implementation Strategy

### MVP First (User Stories 1 & 4 Only)

1. Complete Phase 1: Setup
2. Complete Phase 2: Foundational
3. Complete Phase 3: User Story 1 (Universe)
4. Complete Phase 4: User Story 4 (Characters)
5. **STOP and VALIDATE**: Sufficient for Book 1 writing to begin

### Full Series Planning

1. Complete MVP (US1 + US4)
2. Complete Phase 5: User Story 3 (Mechanics)
3. Complete Phase 6: User Story 2 (Plot)
4. Complete Phase 7: Polish
5. **All planning documents complete**

### Parallel Work Strategy

With multiple contributors:

1. Complete Setup + Foundational together
2. Split work:
   - Contributor A: US1 (Universe Bible)
   - Contributor B: US4 (Characters)
3. After P1 stories complete:
   - Contributor A: US3 (Mechanics)
   - Contributor B: US2 (Plot)
4. Polish phase together

---

## Task Summary

| Phase | User Story | Task Count | Parallel Tasks |
|-------|------------|------------|----------------|
| 1 | Setup | 7 | 5 |
| 2 | Foundational | 4 | 0 |
| 3 | US1 (P1) | 17 | 11 |
| 4 | US4 (P1) | 18 | 6 |
| 5 | US3 (P2) | 20 | 0 |
| 6 | US2 (P2) | 27 | 8 |
| 7 | Polish | 12 | 2 |
| **Total** | | **105** | **32** |

---

## Notes

- [P] tasks = different files, no dependencies within that phase
- [Story] label maps task to specific user story for traceability
- Each user story should be independently completable and validatable
- Validate against contract checklists after each phase
- Commit after each task or logical group
- Stop at any checkpoint to validate story independently
- Constitution principles must be checked especially for Principles I (Tone) and V (Mechanics Integrity)
