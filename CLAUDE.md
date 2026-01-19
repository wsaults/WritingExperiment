# WritingExperiment: LitRPG Universe Project

## Project Overview

A multi-novel LitRPG series featuring **Marcus Chen**, a 33-year-old software engineer thrust into an alien entertainment system where planetary populations compete in survival games broadcast across the galaxy. Tone: **action-comedy** with dark humor, witty banter, and meaningful stakes.

**Genre**: LitRPG (game mechanics integrated into narrative)
**Target**: 5-book series, one standalone dungeon per novel
**Tone Reference**: Dungeon Crawler Carl (dark comedy, irreverent, profane but purposeful)

## Critical Documents

### Governance
- **Constitution**: `.specify/memory/constitution.md` - 7 immutable principles that govern all creative decisions

### Specifications
- **Spec**: `specs/001-litrpg-universe/spec.md` - full feature specification
- **Contracts**: `specs/001-litrpg-universe/contracts/` - deliverable requirements

### Universe Content
- **Bible**: `universe/bible/` - cosmology, species, factions, history, glossary
- **Characters**: `universe/characters/` - protagonist, companions, antagonists, supporting cast
- **Mechanics**: `universe/mechanics/` - stats, classes, skills, economy, system rules
- **Style**: `universe/style/` - voice guide, tone guide, prose examples
- **Plot**: `universe/plot/` - series arc and per-book outlines

## Core Principles (from Constitution)

1. **Action-Comedy Tone** - Violence for entertainment, stakes without grimdark, humor that enhances rather than interrupts
2. **Voice Consistency** - Protagonist: profane, sarcastic, self-deprecating, technically-minded
3. **Protagonist Identity** - Marcus Chen: SWE/robotics background, pattern recognition, systems thinking
4. **Standalone Dungeons** - One unique dungeon per novel, fresh settings prevent fatigue
5. **Mechanics Integrity** - Internal consistency, trackable progression, no retcons
6. **Plot Architecture** - Per-novel resolution + series revelation, escalating stakes
7. **Authenticity** - Write from genuine vision, not market trends

## Working with This Codebase

### Before Creating Content
1. Check relevant contract in `specs/001-litrpg-universe/contracts/`
2. Review constitution principles in `.specify/memory/constitution.md`
3. Cross-reference existing universe content for consistency

### Voice Checklist (Protagonist Marcus Chen)
- [ ] Profane but precise (swearing as punctuation, not filler)
- [ ] Sarcastic observations stated flat, no explained jokes
- [ ] Self-deprecating (targets self before others)
- [ ] Technical analogies in stress/analysis moments
- [ ] Dark humor escalates with danger level
- [ ] Vulnerability rare and brief

### Tone Checklist
- [ ] 70% action/plot, 20% comedy (integrated), 10% character beats
- [ ] Comedy enhances action, doesn't interrupt
- [ ] Deaths quick and impactful, not lingered upon
- [ ] Victories satisfying, not undermined by jokes

### Mechanics Checklist
- [ ] Stats referenced match `universe/mechanics/stats.md`
- [ ] Skills use consistent terminology
- [ ] System interface follows established format
- [ ] Progression feels earned (setup + cost)

## File Naming Conventions

- Species: `universe/bible/species/{species-name}.md`
- Factions: `universe/bible/factions/{faction-name}.md`
- Characters: `universe/characters/{type}/{name}.md`
- Book outlines: `universe/plot/book-{n}/outline.md`

## Terminology

- **The System** - Omnipresent AI governing game mechanics (sardonic personality)
- **Contestants** - Humans and others competing in survival games
- **Dungeons** - Self-contained challenge environments with unique rules
- **The Consortium** - Primary faction running the entertainment industry
- **The Archive** - Repository of all contestant consciousnesses who've died

## Quick Reference: Marcus Chen

- **Age**: 33 at series start
- **Background**: UC Berkeley CS, Stanford robotics dropout, startup lead architect
- **Personality**: Analytical, functional pessimist, emotionally guarded
- **Coping**: Dark humor → problem-solving → physical action → shutdown
- **Moral lines**: Won't sacrifice companions, won't kill non-hostile humans
- **Voice evolution**: Books 1-2 (defensive) → Book 3 (cracks) → Book 4 (breakdown) → Book 5 (integration)
