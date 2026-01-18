# Research: Multi-Novel LitRPG Universe

**Branch**: `001-litrpg-universe` | **Date**: 2026-01-17
**Purpose**: Resolve unknowns and establish foundational decisions before detailed design

---

## Genre Analysis: LitRPG Conventions

### Decision: Core LitRPG Elements to Include

**Decision**: Include stats, levels, classes, skills, inventory, and economy as trackable game elements.

**Rationale**: These are table-stakes for the LitRPG genre. Readers expect to follow progression, theorize about builds, and engage with mechanical decisions. Omitting any creates reader disappointment.

**Alternatives Considered**:
- Minimal mechanics (stats only): Rejected—loses theorycraft appeal
- Maximum crunch (detailed numbers): Rejected—slows action-comedy pacing
- Hybrid approach: **Selected**—enough detail for engaged readers, skimmable for casual readers

### Decision: System Interface Style

**Decision**: The System communicates via text boxes/notifications in protagonist's vision, with occasional sardonic commentary.

**Rationale**: Text-box notifications are genre standard (DCC, HWFWM, Primal Hunter). Adding personality to the System creates comedic opportunities and potential plot relevance.

**Alternatives Considered**:
- Silent system (pure UI): Rejected—misses comedy potential
- Voice in head: Rejected—too intrusive, blurs protagonist's inner voice
- Sardonic text interface: **Selected**—clean separation, comedy opportunities

---

## Comparable Works Analysis

### Dungeon Crawler Carl (Matt Dinniman)

**Relevant Elements**:
- Alien entertainment premise (humans as contestants)
- Dark humor with genuine stakes
- Sardonic AI companion (Donut the cat)
- Level-based dungeon progression
- Sponsor/audience interaction mechanics

**Differentiation Needed**:
- DCC uses mega-dungeon floors; we use standalone dungeons per novel
- DCC protagonist is former Coast Guard; ours is Software Engineer
- DCC has talking cat; we need different companion type

### He Who Fights With Monsters (Shirtaloon)

**Relevant Elements**:
- Isekai setup (Earth human in game world)
- Essence-based power system
- Faction politics matter
- Long-running series with character development

**Differentiation Needed**:
- HWFWM is portal fantasy; ours is "Earth invaded" scenario
- HWFWM protagonist is Australian hipster; ours is American engineer
- HWFWM tone is more earnest; ours is action-comedy throughout

---

## Structural Decisions

### Decision: Standalone Dungeon Format

**Decision**: Each novel features one primary dungeon with its own theme, rules, and challenges. Protagonist exits dungeon at novel's end.

**Rationale**:
- Fresh settings prevent reader fatigue
- Natural novel boundaries (enter → survive → exit)
- Enables wildly different environments (industrial, organic, abstract, etc.)
- Allows power soft-reset between books via dungeon-specific rules

**Alternatives Considered**:
- Mega-dungeon with floors: Rejected—per clarification session
- Open world with dungeons: Rejected—loses focused survival tension
- Standalone dungeons: **Selected**—matches clarification decision

### Decision: Power Progression Model

**Decision**: Stats and abilities persist between dungeons, but each dungeon introduces unique mechanics/restrictions that reset advantage.

**Rationale**: Readers want to see protagonist grow stronger, but power creep kills tension. Dungeon-specific rules (e.g., "magic suppressed," "solo only," "time pressure") create fresh challenges regardless of accumulated power.

**Alternatives Considered**:
- Full reset each book: Rejected—frustrates reader investment
- Unrestricted growth: Rejected—power creep kills tension
- Persistent + restrictions: **Selected**—best of both worlds

---

## Protagonist Background Research

### Decision: Software Engineering Specialization

**Decision**: Protagonist's SWE background focuses on systems design and automation, with robotics experience adding physical/mechanical intuition.

**Rationale**:
- Systems thinking enables "exploit discovery" moments readers love
- Robotics adds credibility for physical problem-solving
- Avoids "hacker" cliché by focusing on architecture over code
- Provides natural exposition method (protagonist analyzes systems aloud)

**Application Examples**:
- Notices game mechanics have edge cases (like software bugs)
- Recognizes patterns in dungeon design (like system architecture)
- Automates/optimizes resource gathering (like CI/CD pipelines)
- Identifies single points of failure in enemy strategies

### Decision: Pre-Apocalypse Life Situation

**Decision**: Protagonist is mid-career SWE (early 30s), recently divorced or relationship-ended, working at a robotics startup. Not at rock bottom, but at a crossroads.

**Rationale**:
- Old enough for competence, young enough for growth
- Relationship baggage provides emotional depth without overwhelming
- Startup context explains broad skill set and adaptability
- "Crossroads" state makes cosmic intervention feel like dark irony, not punishment

**Alternatives Considered**:
- College student: Rejected—less credible competence
- Retired veteran: Rejected—too common in LitRPG
- Happy family man: Rejected—tragedy too heavy for action-comedy
- Directionless crossroads: **Selected**—relatable, not grimdark

---

## Tone Calibration

### Decision: Action-Comedy Balance

**Decision**: 70% action/plot, 20% comedy, 10% character moments. Humor integrated throughout rather than isolated comic relief sections.

**Rationale**: Action-comedy means comedy enhances action rather than interrupting it. Character moments are brief but impactful—earned laughs and earned feelings.

**Implementation**:
- Protagonist's internal monologue provides constant commentary
- Tense situations get tension-breaking quips (not tension-destroying)
- Deaths are quick and consequential, not lingered upon
- Victories are celebrated with dark humor, not speeches

### Decision: Violence Treatment

**Decision**: Violence is exciting and consequential but not gratuitous. Deaths happen, injuries matter, but descriptions focus on action rather than suffering.

**Rationale**: Action-comedy requires stakes but not trauma porn. Readers should feel "oh shit" not "oh god."

**Examples**:
- "His arm came off. That was going to be a problem."
- NOT: "He screamed as tendons tore and blood sprayed..."
- Combat described in tactical terms with emotional beats
- Monster deaths can be more graphic (less empathy required)

---

## Universe Mechanics Research

### Decision: Why Aliens Find Humans Entertaining

**Decision**: Humans are uniquely creative/unpredictable due to short lifespans and survival instincts. Long-lived aliens find human desperation and innovation fascinating—like watching speedrunners.

**Rationale**: Provides in-universe justification for protagonist's unconventional solutions being rewarded. Also explains why Earth was selected (cultural diversity, adaptive species).

### Decision: Game Economic Model

**Decision**: Games are funded by betting markets, sponsor investments, and entertainment subscriptions. Factions compete for profitable contestants.

**Rationale**: Creates multiple stakeholder tensions beyond survival. Protagonist can be manipulated by economic incentives, sponsors have mixed motives, system has ratings pressure.

---

## Open Items Resolved

All NEEDS CLARIFICATION items from spec have been addressed:
- ✅ Protagonist gender: Male
- ✅ Protagonist background: SWE/Robotics
- ✅ Dungeon structure: Standalone per novel
- ✅ Tone: Action-comedy

No remaining unknowns requiring resolution before Phase 1 design.
