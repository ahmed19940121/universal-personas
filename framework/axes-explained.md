# The Two Axes, In Depth

> *The whole framework rests on two questions. Get these two right and the personas fall out naturally.*

This document explains why the framework uses the axes it does, what each end of each axis actually means in practice, and why **'centre'** is a valid (and important) position for one of the five personas.

---

## The inheritance

Cliff Simpkins' original [dev-personas](https://github.com/cliff-simpkins/dev-personas) framework plots developer personas on two axes:

- **Innovation inclination** — how eager a developer is to adopt new technology
- **Decision-making power** — whether they're an individual contributor or a leader

Those axes work beautifully for developer marketing. They don't generalise. "Innovation inclination" is strange to ask about a novelist, and "decision-making power" isn't a useful question for a solo freelancer or a student. We need axes that describe **how a person wants to think and work**, not where they sit on an org chart.

So the Universal Human Personas framework swaps both axes for something more portable:

| Original (dev-personas) | Universal (this repo) |
|---|---|
| Innovation inclination | **Inclination towards curiosity** |
| Decision-making power | **Independence / Influence** |

The spatial logic is preserved — quadrants still mean what they did — but the questions now work for anyone operating any tool.

---

## The X axis — Inclination towards curiosity

```
outcome-led  ◀───────────────────────────────▶  curiosity-led
 "finish it"                                    "understand it"
```

### What this axis is really asking

> *When you pick up a new tool, what do you want from it first — a result, or a understanding?*

This is **not** a measure of intelligence, experience, or ambition. An outcome-led user can be brilliant and deeply experienced; they simply value time-to-result. A curiosity-led user can be a beginner; they simply value the scenic route.

### Outcome-led signals
- Asks "can it do X?" rather than "how does it work?"
- Skims documentation looking for the code block
- Uses defaults and moves on
- Frustrated by tools that force choices before giving output
- Wants the tool to have opinions so they don't have to

### Curiosity-led signals
- Asks "what's the model underneath this?"
- Reads documentation linearly, including the philosophy section
- Customises defaults before first use
- Frustrated by tools that hide their internals
- Wants the tool to expose choice so they can form their own opinions

### Why this matters for AI tools
AI tools are unusually bimodal here. The same product needs to serve users who want a magic button *and* users who want to see the prompt, tune the temperature, and understand why the model said what it said. Framework users on the outcome-led side want sensible defaults and a clear "good enough" path. Framework users on the curiosity-led side want transparency, inspectability, and room to experiment.

---

## The Y axis — Independence / Influence

```
         independent
              ▲
              │
              │
              ▼
        collaborative
```

### What this axis is really asking

> *When you think, do you think alone, or do you think by talking?*

Again, this is **not** a measure of seniority or introversion/extraversion. Some very senior people are deeply collaborative thinkers. Some junior people prefer to work things out alone before speaking. The axis describes *process*, not *position*.

### Independent signals
- Drafts, then shares; rarely shares a half-formed idea
- Uses AI as a reference or a rubber duck, not a partner
- Wants long, complete responses they can read whole
- Finds back-and-forth exhausting for simple requests
- Happy to be left alone with a tool for an afternoon

### Collaborative signals
- Thinks in dialogue, often with an AI as the second voice
- Uses AI as a partner, verbally or near-verbally
- Prefers short turns with frequent course corrections
- Finds a single wall of text harder than five exchanges
- Wants to be met where they are, not handed a finished document

### Why this axis earned its place
This replaced "decision-making power" because the original axis only made sense inside an org chart. Independence / Influence works for a solo founder, a staff engineer, a freelance journalist, and a PhD student — all of whom sit in very different org positions but can be identically collaborative or independent in their actual working style. It's the axis that lets the framework travel.

---

## The five positions

| Persona | X (outcome ↔ curiosity) | Y (collab ↔ independent) | Quadrant |
|---|---|---|---|
| 🟣 **Architect** *Adam* | Curiosity-led | Independent | Top-right |
| 🔵 **Explorer** *Elan* | Curiosity-led | Collaborative | Bottom-right |
| 🟠 **Builder** *Bilal* | Outcome-led | Independent | Top-left |
| 🩷 **Connector** *Cora* | Outcome-led | Collaborative | Bottom-left |
| 🟢 **Steady** *Soren* | Outcome-led | **Centre** | Mid-left |

---

## Why Soren is in the centre

Four of the five personas sit at the corners of the grid. Soren — the Steady — sits in the middle of the Y axis, still clearly on the outcome-led side of the X axis but neither fully independent nor fully collaborative.

This is deliberate.

The Steady is **the largest real-world population** of any of the five, and the population most often missed by persona frameworks. They are the people who adopt a tool once the early adopters have de-risked it, who want it to work, who will defect to a competitor silently if it doesn't, and who describe themselves with phrases like *"I'm not really a tech person."*

Soren isn't centre because they're an average of the other four. Soren is centre because their **defining behaviour is refusing to commit to a corner**. They want:

- A proven, safe choice (not innovation for its own sake — Builder-adjacent)
- Some support and reassurance (not solo heroics — Connector-adjacent)
- But not so much back-and-forth that it slows them down (not Explorer-like dialogue)
- And definitely not a customisation rabbit hole (not Architect-like depth)

The centre is the position that says *"I want the tool to meet me in the middle."* That's a real, populous, underserved archetype, and the framework would be incomplete without it.

---

## What this framework deliberately leaves out

The axes make some things **visible** and some things **invisible**. It's worth being explicit about the trade-off:

**Visible**
- How someone wants to think (alone vs. with)
- What they want from a tool (outcome vs. understanding)
- Where they'll feel served or frustrated by a given design choice

**Invisible — by design**
- Job title, seniority, tenure
- Technical skill level
- Domain expertise
- Demographic variables
- Organisation size

The invisibles don't disappear — they show up when you apply sub-personas. Builder's sub-persona set (Bayo, Bilal, Brynn, Benedict, Blake) holds Builder's axis position constant and varies the *context*: student, professional, founder, domain specialist, no-code operator. Each parent persona can be refined the same way.

This keeps the **top-level model** clean and portable, while the sub-personas carry the contextual weight.

---

## Using the axes as a design prompt

When you're making a decision about a feature, a piece of content, or a sales motion, pick the axes up and hold them against the decision:

1. *Which axis position does this serve?*
2. *Which axis positions does it actively exclude?*
3. *Is the exclusion deliberate or accidental?*

Accidental exclusion is how products end up serving only Architects and Explorers (the loud, curious, online half of the map) while quietly alienating Builders, Connectors, and Steadies (the quiet, outcome-focused, offline half). The framework is most useful as a check against that drift.
