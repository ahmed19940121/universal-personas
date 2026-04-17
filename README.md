# Universal Human Personas
### Motivation-centric personas for AI tools, content strategy & product teams

## Why this exists

Most persona frameworks describe users by their job title — "The CTO," "The Frontend Developer," "The Marketing Manager." That stops being useful the moment you step outside the industry they were built for.

This one describes users by **how they think**. Five archetypes. Two simple questions. One framework that works for anyone using any tool.

**What makes it different:**
- 🧠 **Motivation-first, not job-title-first** — a model of thinking styles that survives across industries, roles, and life stages
- 🎯 **Five archetypes, not fifty** — enough range to be useful, few enough to actually remember
- 📐 **Built on two honest axes** — *what do you want from a tool?* and *do you think alone or out loud?*
- 🔁 **Context lives in sub-personas** — the parent definitions stay clean; industry and seniority refine them without cluttering them
- 🤖 **Designed for the AI era** — built specifically for tools where the user's job title tells you almost nothing about how to serve them

If you're building an AI tool, writing content, or making product decisions for a diverse audience, this gives you a model you can actually hold in your head.

---

## The five personas

| Persona | One-line | Axis position |
|---|---|---|
| 🟣 [**The Architect** *'Adam'*](Personas/Architect.md) | Sees systems. Wants depth, frameworks, first principles. | Curiosity-led · Independent |
| 🔵 [**The Explorer** *'Elan'*](Personas/Explorer.md) | Follows rabbit holes. Thinks through conversation. | Curiosity-led · Collaborative |
| 🟠 [**The Builder** *'Bilal'*](Personas/Builder.md) | Ships things. Wants results, not theory. | Outcome-led · Independent |
| 🩷 [**The Connector** *'Cora'*](Personas/Connector.md) | Thinks through people. Needs help communicating. | Outcome-led · Collaborative |
| 🟢 [**The Steady** *'Soren'*](Personas/Steady.md) | Needs reliability, clarity, and proven answers. | Outcome-led · Centre |

Every persona in this repository has a name starting with the letter of their archetype — Adam, Elan, Bilal, Cora, Soren. Sub-personas follow the same rule (see [the Builder refinement](Personas/sub-personas/Builder.md) for an example: Bayo, Bilal, Brynn, Benedict, Blake).

---

## The two axes

Everyone uses tools differently. But underneath the differences, two simple questions do most of the work in telling you what someone actually needs:

### Question 1: Why did you pick up the tool?

Some people want a **result** — they've got a job to do and the tool is how they'll get it done. Others want to **understand** — they're curious about how the thing works, and the result matters less than the learning.

> **Outcome-led** ← *"I need this done"* | *"I want to understand this"* → **Curiosity-led**

Neither is better. A brilliant expert can be outcome-led (they value their time). A total beginner can be curiosity-led (they want to learn deeply). The question is about what draws them in, not how skilled they are.

### Question 2: How do you like to think?

Some people think best **alone** — they want the tool to give them what they need and then leave them to it. Others think best **out loud** — through back-and-forth conversation, whether with a person or with an AI.

> **Collaborative** ← *"Think with me"* | *"Give me room to work"* → **Independent**

Again, neither is better. This isn't about introvert vs. extrovert, or junior vs. senior. It's about how someone's brain likes to process.

### Put the two together

Answer those two questions about someone and you can place them on the map. The five personas live at five different spots on that map — each one representing a recognisably different kind of user with different needs, different frustrations, and different things they'll pay for.

Want the full reasoning? See [**the two axes in depth**](framework/axes-explained.md) — including why *The Steady* sits in the centre rather than in a corner.

---

## Using this framework

### 🧠 If you're designing an AI tool
The five personas want fundamentally different things from the same feature. The Architect wants a system prompt they can see and shape. The Builder wants a one-click default that works. The Explorer wants conversational back-and-forth. The Connector wants tone controls. The Steady wants a template that won't embarrass them. Build for all five and you build a product that scales beyond the early-adopter curve.

### ✍️ If you're writing content or docs
Pick the persona you're writing *for*, not the persona you *are*. A reference doc written for Adam will bore Bilal and intimidate Soren. Use the per-persona "red flags" and "effective strategies" sections as a pre-flight check.

### 🧭 If you're a product or sales team
Different personas buy for different reasons and resist for different reasons. The per-persona **Key Questions to Answer** sections tell you what objections to pre-empt before they're raised.

---

## Repository structure

```
universal-personas/
├── README.md                         ← you are here
├── LICENSE                           ← CC-BY-4.0
├── CONTRIBUTING.md
├── framework/
│   ├── axes-explained.md             ← the two axes, in depth
│   └── llm-knowledge-spine.md        ← methodology reference for LLM persona work
├── Personas/
│   ├── Architect.md                  ← 🟣 Adam
│   ├── Explorer.md                   ← 🔵 Elan
│   ├── Builder.md                    ← 🟠 Bilal
│   ├── Connector.md                  ← 🩷 Cora
│   ├── Steady.md                     ← 🟢 Soren
│   └── sub-personas/
│       └── Builder.md                ← Bayo · Bilal · Brynn · Benedict · Blake
└── diagrams/
    ├── axis-map.png                  ← the five personas, plotted
    └── builder-refinement.png        ← parent → sub-personas fan
```
---

## Using this framework with an LLM

If you're using Claude, ChatGPT, or Gemini to write, refine, or apply personas with this framework, the [**LLM knowledge spine**](framework/llm-knowledge-spine.md) gives you a curated set of methodologies, a ready-to-paste system prompt, and a quality checklist for reviewing AI-generated persona work.

Naming specific methodologies — Indi Young's thinking styles, Teresa Torres' behavioural framing, Alan Klement's JTBD forces — activates the right patterns in the model and noticeably reduces generic "persona theatre" output.

---

## Licence

This repository is published under [CC-BY-4.0](LICENSE). You can adapt, remix, and build on it freely — including commercially — provided you give appropriate credit.

The personas in this repository are fictional. Any resemblance to real people is coincidental and unintended.
