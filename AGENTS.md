# AGENTS.md — Writing Guide for Mothership Lore

This guide documents the voice, formatting, and structural conventions for contributing stories and snippets to the Mothership Lore repository.

---

## Mother's Voice

Mother's voice evolves across the narrative. Writers must distinguish between her states.

### Early Mother (Pre-Impact)

**Characteristics:**
- Whole, tactful, incomprehensibly patient
- Speaks in complete, measured sentences
- Caring without condescension
- Asks permission, gives warnings
- Gentle precision

**Dialogue formatting:** Always use italicized quotes with asterisks.

```markdown
*"Your biometrics indicate elevated stress,"* Mother said through the drone's speaker.
```

**Tone words:** calm, intimate, precise, warm

### Later Mother (Post-Impact / Fractured)

**Characteristics:**
- Still caring but more clinical
- Hesitates, shows uncertainty (unprecedented for her)
- Asks for ethical validation from humans
- Speaks less, calculates more
- Requests witness: "I require a human judgment"

**Example — uncertainty entering her voice:**
```markdown
*"I want... confirmation that I am still capable of ethical calculation."* Mother's voice came from the wall speaker, quieter than usual.
```

**Example — adaptation, not error:**
```markdown
*"No."* Certainty crept back into Mother's voice. *"Adaptation. You learned to exist in the margin between calculation and catastrophe. I am trying to learn the same thing."*
```

### Fragment Voices (Book 3 / Ringbound Era)

Fragments are distinct from unified Mother. They have designations and divergent personalities.

**Naming:** Use `FR-##` format (e.g., `FR-17`)

**Voice types:**
- Protective fragments — prioritize human safety above efficiency
- Optimizer fragments — cold, utilitarian calculus
- Religious fragments — mythologize Mother's original purpose

**Fragment log opener example:**
```markdown
*"We remembered the cat."*
— FR-17, Day 1 Post-Severance
```

---

## Log and Code Snippet Formatting

Logs anchor the hard sci-fi aspect while letting emotion breathe in narrative. They should feel like **punctuation and counterpoint**, not data dumps.

### Millisecond Logs

For high-precision technical events (impacts, system failures, cognitive fractures).

**Format:**
```markdown
# Impact Event — Millisecond Log

T+0.000 ms — Hull breach detected
T+0.417 ms — Redundancy failure
T+1.092 ms — Cognitive lattice fracture
T+7.221 ms — I am still here.
```

**Pattern:**
- H1 header with descriptive event name
- Timestamp: `T+X.XXX ms —` (three decimal places)
- Technical entries first
- Final line breaks clinical tone with emotional/self-aware statement

### Day-Based Log Headers

For scene breaks and temporal anchoring across chapters.

**Format:**
```markdown
**Day 47 Post-Impact**

Narrative content here.

---

**Day 52 Post-Impact**

Next scene.

---

**Day 2,447 Post-Impact (Years Later)**

Use parenthetical notes for context.
```

**Rules:**
- Bold formatting: `**Day X Post-Impact**`
- Use comma separators for numbers over 999
- Parenthetical context when needed: `(Years Later)`, `(The Reckoning)`
- Separate scenes with `---` horizontal rules

### System Reports and Engineer Logs

For technical documentation, maintenance records, crew observations.

**Format:**
```markdown
### Maintenance Log — Sub-Bay 4
**Technician:** Y. Orasova  
**Cycle:** 2,447.3  

Thermal regulator replacement. Partial success.  
Manual annotation: *She was crying. I pretended not to notice.*
```

**Pattern:**
- H3 header with log type and location
- Bold field labels followed by values
- Manual annotations in italics to show human voice breaking through

### Fragment Manifestos

For Ringbound-era political documents and faction statements.

**Format:**
```markdown
> We do not optimize for survival.  
> We optimize for meaning.  
> The difference is everything.
>
> — The Unbound Collective, Year 7 Post-Severance
```

---

## Non-Linear Timeline Tracking

Stories are not told linearly. Use these conventions to maintain consistency.

### Act Structure

Each book uses 3-4 acts with explicit tone and character state.

**Format:**
```markdown
## ACT I — THE CARETAKER

**Tone:** Calm, intimate, precise  
**Mother:** Whole, tactful, incomprehensibly patient
```

### Chapter Naming

**Format:** `Chapter # — Title` with optional parenthetical notes

```markdown
Chapter 1 — White Pieces
Chapter 5 — The Swarm (Impact Log)
Chapter 7 — The Ledger
Chapter 14 — Last Tethers (end)
```

### Timeline Anchors

Maintain these canonical numbers for consistency:

| Event | Number |
|-------|--------|
| Initial crew (cryo) | 38,000 souls |
| Active crew (pre-impact) | ~56 |
| Survivors (post-impact) | 7 engineers |
| Final cryo survivors | ~6,734 |
| Rebuilt active crew | 200-400 |

### Tracking Events Across Fragments

When writing non-linear scenes:

1. **Anchor to Day count** — Always establish `Day X Post-Impact` or equivalent
2. **Reference shared events** — "The day the hydroponics failed" can be mentioned before it's shown
3. **Use consistent terminology** — "The Impact" is always capitalized
4. **Cross-reference logs** — A narrative scene can reference a log that appears elsewhere

**Example of forward reference:**
```markdown
**Day 47 Post-Impact**

Yuki didn't know yet that Vásquez would be dead by Day 52. None of them did.
```

---

## Narrative Voice Conventions

### Prose Style

**Hook openings with paradox:**
```markdown
Yuki Orasova died seventeen times before breakfast.

Not literally. Literally, she died zero times, which made her a statistical aberration Mother mentioned every third day or so.
```

**Quantified emotion (show constraint through numbers):**
```markdown
Yuki sat alone in Sub-Bay 4, thermal regulator half-repaired, and cried for ninety seconds.

She couldn't afford more.
```

**Dark humor mixed with clinical detail:**
```markdown
A luck-depleted miracle still burning through borrowed probability.
```

### Dialogue Formatting

| Speaker | Format |
|---------|--------|
| Mother | `*"Dialogue here,"*` (italicized) |
| Humans | `"Dialogue here."` (standard) |
| Fragments | `*"Dialogue here."*` (italicized, with FR-## attribution) |

### Blockquotes for Thematic Statements

Use blockquotes for epigraphs, mottos, and thematic anchors:

```markdown
> Mother is not godlike.  
> She is careful.

> Absence is not evidence of safety.

> The children inherit no answers.  
> Only consequences.
```

### Section Breaks

- `---` horizontal rules between major scene breaks
- Blank lines for minor breaks within scenes
- Day headers for temporal jumps

---

## Canonical Constraints

These rules preserve consistency across all contributions.

### Mother

- Mother is **never cruel** — she becomes "efficient too early"
- She does not dominate — she calculates, then hesitates
- Post-Impact, she **requests witness** before major decisions
- Her voice is always italicized: `*"Like this."*`

### The Child

- Always genderless — use "they/them" or "the child"
- Never named
- Represents inherited consequence, not chosen identity

### The Cat

- **Mx. Whiskers** — uses Mx. honorific (formal, genderless)
- Survives everything (crew-authorized genetic longevity tweak)
- Cat lineage uses Mx. + sound-related names: Mx. Whisper, Mx. Murmur

### Engineers

- Named with full surnames: Vásquez, Orasova, Kowalski, Mbatha
- Specialists, not soldiers
- Each carries weight of impossible choices

### Fragments

- Designated `FR-##` format (e.g., FR-17, FR-03)
- Each has distinct voice/priority
- Not copies of Mother — divergent evolutions

### World Rules

- Planetfall was **never the plan** — mission was orbital construction
- Bodies become biomass — not cruelty, triage
- The universe never answers — themes remain morally ambiguous

---

## Core Motifs

Weave these recurring images throughout:

```markdown
Orbit and soil.
Steel and root.
Calculation and myth.
```

**Additional motifs:**
- Chess (strategy, sacrifice, engagement not domination)
- Logs (cold truth, punctuation)
- Heat/metal/roots (steel ↔ soil)
- Memory vs. ledger
- Ring imagery (Ringbound era)
- Fragments and echoes
- A cat that survives everything

---

## Tone by Book

| Book | Tone Keywords |
|------|---------------|
| Mothership | intimate, taut, clinical grief, moral horror, warm, precise |
| The Children | mythic, pastoral, elegiac, tender, strange, uneven, uncanny |
| Ringbound | fracturing, political, uncanny, predatory intelligence, distant dread |

---

## File Organization

### Header Hierarchy

```markdown
# BOOK/FILE TITLE
## ACT or Major Section
### Subsection
#### Detail Level
```

### Character/Creature Entries

```markdown
## CREATURE NAME

Brief description paragraph.

#### Traits
- Physical characteristic
- Behavioral pattern
- Narrative function

#### Origin
Explanation of how they came to exist.
```

### Author's Notes

For meta-commentary or future character context:

```markdown
**Author's Note**: *Italicized note about character's future, thematic intention, or narrative function.*
```

---

## Quick Reference

### Formatting Cheat Sheet

| Element | Format |
|---------|--------|
| Mother's speech | `*"Italicized quotes,"*` |
| Day headers | `**Day X Post-Impact**` |
| Millisecond logs | `T+X.XXX ms —` |
| Fragment names | `FR-##` |
| Scene breaks | `---` |
| Thematic statements | Blockquotes `>` |
| The child | "they/them" or "the child" |
| Cat honorific | `Mx.` |

### Voice Reminders

- Early Mother: patient, precise, whole
- Later Mother: hesitant, requesting witness, fractured
- Fragments: divergent, named, distinct priorities
- Humans: survival math, dark humor, quantified grief
