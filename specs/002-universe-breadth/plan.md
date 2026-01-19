# Implementation Plan: Universe Breadth Expansion

**Branch**: `002-universe-breadth` | **Date**: 2026-01-19 | **Spec**: [spec.md](./spec.md)
**Input**: Feature specification from `/specs/002-universe-breadth/spec.md`

## Summary

Expand the LitRPG universe documentation from 5 species to approximately 100 species across three detail tiers, complete all 12 founder species profiles, document humans from galactic perspective, add human survivor culture/settlements, expand Books 2-5 dungeon designs to match Book 1 depth, enhance economy/item documentation, and create galactic geography reference. All content follows established constitution principles and existing glossary terminology.

## Technical Context

**Content Type**: Creative worldbuilding reference documentation (Markdown)
**Language/Version**: Markdown with established formatting conventions from existing universe files
**Primary Dependencies**: Existing universe bible (`universe/bible/`), character files, mechanics docs
**Storage**: Git repository, Markdown files organized by category
**Testing**: Manual validation against success criteria; cross-reference checks against glossary
**Target Platform**: Author reference material (human readable Markdown)
**Project Type**: Documentation expansion (single repository, no code)
**Performance Goals**: N/A (reference documentation)
**Constraints**: Constitution principles, existing terminology, narrative consistency
**Scale/Scope**: ~100 species profiles, 12 founder species, 4 dungeon expansions, 1 geography doc, 1 economy expansion, 3 human settlement types, 3 human factions

## Constitution Check

*GATE: Must pass before Phase 0 research. Re-check after Phase 1 design.*

| Principle | Status | Verification |
|-----------|--------|--------------|
| I. Action-Comedy Tone | PASS | Species attitudes, faction descriptions maintain tone guidance |
| II. Character Voice Consistency | PASS | N/A for worldbuilding docs; character docs follow voice rules |
| III. Protagonist Identity | PASS | Human species entry written from alien perspective, not protagonist POV |
| IV. World Structure: Standalone Dungeons | PASS | Dungeon expansions maintain one-dungeon-per-book principle |
| V. Game Mechanics Integrity | PASS | Economy/item expansion consistent with established mechanics |
| VI. Plot Architecture | PASS | Founder species support series plot; Thirteenth Founder mystery preserved |
| VII. Authenticity Over Trend-Chasing | PASS | D&D inspiration adapted to sci-fi, not direct ports |

**Gate Result**: PASS - No violations. Proceed to Phase 0.

## Project Structure

### Documentation (this feature)

```text
specs/002-universe-breadth/
├── plan.md              # This file
├── research.md          # Phase 0 output
├── data-model.md        # Phase 1 output (species taxonomy, file structure)
├── quickstart.md        # Phase 1 output (how to use expanded universe)
├── contracts/           # Phase 1 output (file format contracts)
│   ├── species-tier1.md # Tier 1 species file format
│   ├── species-tier2.md # Tier 2 species file format
│   ├── species-tier3.md # Tier 3 species file format
│   └── master-index.md  # Species index format
└── tasks.md             # Phase 2 output (/speckit.tasks command)
```

### Source Content (repository root)

```text
universe/
├── bible/
│   ├── species/
│   │   ├── founders/           # All 12 founder species (Tier 1)
│   │   │   ├── velthrani.md    # Existing, to be enhanced
│   │   │   └── [11 new founders].md
│   │   ├── major/              # Plot-critical non-founders (Tier 1)
│   │   │   ├── kindari.md      # Existing, reclassified
│   │   │   ├── quorathi.md     # Existing, reclassified
│   │   │   ├── thex-collective.md # Existing, reclassified
│   │   │   ├── vorrax.md       # Existing, reclassified
│   │   │   ├── humans.md       # NEW - galactic perspective
│   │   │   └── [3-5 new major].md
│   │   ├── recurring/          # Faction-affiliated, named characters (Tier 2)
│   │   │   └── [30-35 species].md
│   │   ├── background/         # Scene population variety (Tier 3)
│   │   │   └── [45-50 species].md
│   │   └── index.md            # Master species index
│   ├── factions/               # Existing, no changes planned
│   ├── geography/              # NEW directory
│   │   └── galactic-regions.md # Major regions and travel context
│   ├── cosmology.md            # Existing, reference only
│   ├── history.md              # Existing, reference only
│   └── glossary.md             # Existing, to be updated with new terms
├── characters/
│   └── [existing structure unchanged]
├── mechanics/
│   ├── economy.md              # Existing, to be expanded
│   ├── items/                  # NEW directory
│   │   └── item-catalog.md     # Example items by tier
│   └── [other existing files unchanged]
├── plot/
│   ├── book-1/dungeon-design.md  # Existing (2,100 words) - reference
│   ├── book-2/dungeon-design.md  # Existing, to be expanded
│   ├── book-3/dungeon-design.md  # Existing, to be expanded
│   ├── book-4/dungeon-design.md  # Existing, to be expanded
│   └── book-5/dungeon-design.md  # Existing, to be expanded
└── culture/                    # NEW directory
    ├── human-settlements.md    # 3 settlement types
    └── human-factions.md       # 3+ faction philosophies

```

**Structure Decision**: Expand existing `universe/` directory structure with new subdirectories for species tiers, geography, items, and human culture. Maintains existing organization patterns while accommodating ~100 species across clear tiers.

## Complexity Tracking

> No violations requiring justification. All content follows existing patterns.
