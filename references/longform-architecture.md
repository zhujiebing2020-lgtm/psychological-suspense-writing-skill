# Longform Architecture

Use this when planning or reviewing an 18-23万字 psychological suspense novel, a 20-30 installment serial, or any longform mystery where clue management and relationship progression must both hold.

## Core Judgment

Long psychological suspense can only sustain length if every installment carries more than plot discovery.

Each installment needs:

- one suspense movement
- one relationship scene
- one body/mental pressure node
- one viewpoint texture
- one delayed return or future hook

If an installment only reveals evidence, it becomes thin.

If it only explains emotion, it becomes stagnant.

## Installment Budget

For 18-23万字:

- 20 installments: 9,000-11,500 Chinese characters each
- 23 installments: 7,800-10,000 Chinese characters each
- 27 installments: 6,700-8,500 Chinese characters each
- 30 installments: 6,000-7,700 Chinese characters each

Do not force identical length. Major confrontations, corpse/body reveals, and final reversals can run longer.

## Three-Act Load

### Act One: Disappearance / Disturbance / First System

Function:

- establish the investigator's wound and method
- introduce the first body clue or symbolic object
- present an apparent relationship story
- reveal that the case is not ordinary

Risks:

- too much protagonist viewpoint
- too much clue labeling
- theme stated too early

Counterweights:

- witness material
- procedural pressure
- small fragments of the missing/dead person

### Act Two: Body / Relationship / Contradiction

Function:

- deepen body clues
- reveal active harm by sympathetic characters
- make the central absent/dead/missing person complex
- move from "who did it" toward "what was everyone doing to this person"

Risks:

- middle sag
- repeated confrontations
- everyone talking about the absent person rather than scenes making them return

Counterweights:

- external investigation pressure every 2-3 installments
- one concrete past scene per major relationship turn
- recurring body clues with changed meaning

### Act Three: Wound / Display / Ethical Reckoning

Function:

- make the hidden system visible
- reveal the protagonist's moral implication if relevant
- recover withheld relationship meanings
- convert the final body/object/place into a mirror of the whole book

Risks:

- overexplaining the antagonist
- procedural implausibility
- final theme becoming a lecture

Counterweights:

- concrete path ledger for the final reveal
- limited antagonist viewpoint
- final images and actions over final thesis

## Viewpoint Budget

A useful default:

- primary viewpoint: 45-60%
- witness/love/rival viewpoint: 10-20%
- procedural viewpoint: 8-12%
- absent/dead/missing person fragments: 8-15%
- antagonist: 3-8%
- side witnesses/family/experts: 5-10%

Rule:

The primary viewpoint is the spine. Other viewpoints are cracks.

## Body Node Ledger

Every major body node or object motif should return at least three times:

1. early trace
2. middle contradiction
3. late reversal

Example:

- early: a hand blocks a camera
- middle: a hand mold, wound, or ring reframes the gesture
- late: a final arranged hand reveals the loss of agency

## Relationship Scene Reservoir

When an installment is thin, add one of these:

- someone gently hurting another person through care
- someone solving a problem before the other person can decide
- someone making honesty feel like pressure
- someone naming violation as protection or repair
- a procedural character forcing evidence-source clarity
- an archive keeper refusing clean interpretation
- an absent person designing exits while losing their own

The scene must change the current chapter, not sit as decoration.

## Publishability Test

Before treating an installment as ready, ask:

- Does it have one complete present scene?
- Does it contain one past scene, memory, recording, or material trace that changes the present?
- Does at least one non-primary perception enter the chapter?
- Does it advance two of suspense, emotion, theme?
- Does the ending hook open one strong question, not five?
- Can the absent/dead/missing person be felt as a person?

## Red Flags

The project is becoming thin if:

- every chapter opens with the protagonist reading a document
- police/procedure only delivers information
- witnesses only explain the past
- initials, symbols, or labels repeat more often than systems
- the missing/dead character appears only as a memory object
- body motifs appear in predictable order
- chapter endings stack multiple discoveries
- theme sentences explain what the image already did

The fix is usually:

add a scene, not an explanation.

## Cross-Chapter Heatmap

Use this trilinear tracking system to expose middle sag before drafting. After outlining or revising, build a heatmap table: each chapter gets three scores (1–10), plus a combined load score. A healthy chapter carries at least two hot lines. When all three lines dip below 4 simultaneously across two or more consecutive chapters, the structure has a sag zone — fix it before writing, not after.

### Trilinear Heatmap Schema

Each chapter records:

| field | what it measures | how to score (1–10) |
|---|---|---|
| `suspense_temp` | how strongly does this chapter advance the mystery? evidence discovered, access gained/lost, timeline tightened, procedural contradiction, reveal or bait-and-switch, delayed return of an old clue | 1 = no evidence movement, 10 = major reveal or irreversible escalation |
| `relationship_load` | how deeply does a relationship change in this chapter? trust broken/rebuilt, power shifted, intimacy weaponized, a character's pressure system forces another to react, a past scene reframes a present bond | 1 = everyone stays in their emotional lane, 10 = a relationship crosses a line it cannot uncross |
| `body_load` | how much does the body register in this chapter? sensation, wound, gesture, medical trace, object contact, environmental pressure, a body clue returns with different meaning, bodily memory disrupts the present | 1 = no physical trace, 10 = a body node becomes irreversible evidence or collapses a prior reading |

### Combined Load Score

```
combined_load = round((suspense_temp × 0.40 + relationship_load × 0.35 + body_load × 0.25), 1)
```

Weights descend because suspense is the genre engine, relationship is the emotional engine, and body is the sensory engine. Adjust for specific projects.

### Heatmap Table Template

```
| ch | title | s_temp | r_load | b_load | comb | viewpoint | notes |
|----|-------|--------|--------|--------|------|-----------|-------|
| 01 |       |        |        |        |      |           |       |
| 02 |       |        |        |        |      |           |       |
...
```

### Sag Detection Rules

A chapter is underloaded when:

- `combined_load < 3.5`
- or `suspense_temp < 3 AND relationship_load < 3`

A sag zone is:

- two or more consecutive chapters with `combined_load < 4.0`
- or three consecutive chapters where `suspense_temp < 4` (evidence starvation)

A false peak is:

- `suspense_temp ≥ 8` but `relationship_load ≤ 3` and `body_load ≤ 3`
- means the chapter reveals evidence without emotional or sensory weight — reads like a report, not a scene

A false peak cluster (two consecutive false peaks) is worse than a sag zone: it trains the reader that reveals are hollow.

### Act-Level Health Check

After scoring the full heatmap, compute act averages:

```
Act One (installments 1–6 or 7): avg suspense ≥ 5.0, avg relationship ≥ 5.5, avg body ≥ 4.5
Act Two (installments 7/8–16/18): avg suspense ≥ 5.5, avg relationship ≥ 5.0, avg body ≥ 5.0
Act Three (final 4–6 installments): avg suspense ≥ 6.0, avg body ≥ 5.5
```

Act Two typically dips 1–2 points across all lines — the sag is structural, not a sign of failure. But the dip must not exceed two consecutive sag-zone chapters without a spike.

### Heatmap-Driven Revision

When the heatmap flags a problem, add a specific scene type rather than padding:

- `suspense_temp` too low: add a procedural detection scene, an evidence-source contradiction, a timeline tightening, or a clue return with new context
- `relationship_load` too low: add a care scene that becomes control, a confrontation with delayed response, a shared memory that reframes current trust, or a truth-demand that feels like pressure
- `body_load` too low: add a body trace (scar, gesture, posture, breath change), a medical or forensic detail, a body-object contact, or a returning bodily memory
- `combined_load` too low across two+ lines: add a scene that forces all three to move simultaneously — e.g. a medical examination that reveals a wound (body), contradicts a prior statement (suspense), and exposes who controls the patient's narrative (relationship)

### Agent Automation

When building a Claude Code agent around this skill, the agent should:

1. After outline or draft, auto-generate a heatmap CSV at `project/heatmap.csv`
2. Flag every sag zone, false peak, and false peak cluster in the output
3. Before writing each chapter, read the heatmap row for the current chapter and the two adjacent chapters
4. After completing a chapter, score the actual chapter against the planned heatmap row: if actual deviates by ≥3 points on any line, note the drift and decide whether to revise the chapter or update the heatmap
5. At act boundaries, run the act-level health check and report underloaded acts

Do not let the heatmap override intuition. A chapter that breaks all rules but reads perfectly is correct. The heatmap only flags structural risk before writing, so the writer can choose to add a scene rather than discover sag after 15 chapters.
