# Universal Human Personas
### Motivation-centric personas for AI tools, content strategy & product teams

> *"A curious independent is a curious independent whether they're writing code, writing copy, or writing a thesis. They want the same kind of thing from the tool in front of them."*

<p align="center">
  <img src="diagrams/axis-map.png" alt="The five Universal Human Personas plotted on two axes: outcome-led to curiosity-led, and collaborative to independent" width="85%"/>
</p>

---

## Why this exists

Andrej Karpathy has a habit of teaching from first principles. When he explains a transformer, he doesn't hand you the API — he rebuilds the thing from scratch, in public, so you end up with a working mental model rather than a list of facts about it. The lesson generalises: *a real model beats any amount of surface knowledge, because the model generates the answers while the knowledge just lists them.*

Persona work has the same property at its best. A great persona isn't a demographic snapshot or a job-title dossier; it's a model of **how someone thinks**, portable enough to apply to any product or context they encounter. Given a clean model, you can derive the surface facts — what they'll tolerate, what will frustrate them, what they'll pay for — without having to memorise them.

Most persona frameworks don't have this property. They're **job-title-centric** — "The CTO," "The Frontend Developer," "The Marketing Manager" — and they stop being useful the moment you step outside the industry they were built for. They also age poorly, because job titles drift faster than human motivations do.

This framework tries to work from first principles instead. Five archetypes, two axes, and a structural rule that context (industry, seniority, domain) lives in sub-personas rather than in the parent definitions. What you end up with is a model you can apply to anyone using any tool — particularly AI tools, content platforms, and new products, where the job title of the user tells you almost nothing useful about how to serve them.

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

<table>
<tr>
<td width="50%">

### X axis — Inclination towards curiosity

**Outcome-led** ◀ ─────────── ▶ **Curiosity-led**

*"I need this done"* ◀ ─── ▶ *"I want to understand this"*

Outcome-led users reach for a tool to finish a task. Curiosity-led users reach for a tool to open a door.

</td>
<td width="50%">

### Y axis — Independence / Influence

**Collaborative** ▼ ─────────── ▲ **Independent**

*"Think with me"* ▼ ───── ▲ *"Give me room to work"*

Collaborative users process by bouncing ideas off others (or an AI). Independent users process alone and want the tool out of their way.

</td>
</tr>
</table>

Read [**the full axes explanation**](framework/axes-explained.md) for the reasoning behind the placements and why "centre" is a valid position for Soren.

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
│   └── axes-explained.md             ← the two axes, in depth
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

## Roadmap

- [x] Five parent personas written in full
- [x] Builder sub-persona set (5 variants)
- [x] Axis map and Builder refinement diagrams
- [ ] Architect sub-personas (Adam, Ari, Asha, Anand, Ada)
- [ ] Explorer sub-personas (Elan, Eli, Esha, Enzo, Eva)
- [ ] Connector sub-personas (Cora, Cai, Cleo, Chen, Caleb)
- [ ] Steady sub-personas (Soren, Sam, Suki, Sana, Stan)
- [ ] Refinement diagrams for the four remaining archetypes
- [ ] Reusable Gemini prompt templates for generating more diagrams in the same style
- [ ] Worked examples: applying the framework to three real products

---

## Further reading

The framework is designed to be useful on its own, but it draws on a long tradition of persona and user-research thinking. If you want to go deeper — or build your own persona work on firmer foundations — these are the books and resources worth your time.

### Books

The persona canon most worth reading, roughly in order of usefulness for this framework:

- **The Mom Test** — Rob Fitzpatrick. How to actually talk to users so they tell you the truth. If you're building personas from interviews, read this first.
- **Continuous Discovery Habits** — Teresa Torres. The best modern treatment of how to keep personas alive as working artefacts rather than dead documents.
- **Practical Empathy** — Indi Young. The deepest available guide to listening sessions and the "thinking styles" approach that informs the curiosity axis in this framework.
- **The Inmates Are Running the Asylum** — Alan Cooper. The origin text for personas in product design. Worth reading for the history, even if the specific methodology has moved on.
- **Designing for the Digital Age** — Kim Goodwin. The Cooper-tradition persona methodology in full, industrial-strength form.
- **Jobs to Be Done: Theory to Practice** — Anthony Ulwick. An important counterpoint to persona-centred design; worth knowing even if you stay persona-first.
- **Hooked** — Nir Eyal. On user motivation and habit formation; useful for filling in the "why" behind persona behaviours.
- **Thinking, Fast and Slow** — Daniel Kahneman. The underpinning model of human decision-making that makes every persona framework richer.

### Online resources

- **Nielsen Norman Group** — [nngroup.com](https://www.nngroup.com) · the most-cited UX research library, with a deep persona-specific back-catalogue
- **Indi Young** — [indiyoung.com](https://indiyoung.com) · especially her writing on listening sessions and thinking styles
- **Product Talk (Teresa Torres)** — [producttalk.org](https://www.producttalk.org) · opportunity-solution trees, continuous discovery, interview practice
- **Jobs-to-be-Done Institute** — [jobs-to-be-done.com](https://jobs-to-be-done.com) · the structured JTBD methodology
- **Andrej Karpathy's lectures** — [karpathy.ai](https://karpathy.ai) · referenced in the motivation above; a worked example of teaching mental models rather than facts
- **Basecamp's Shape Up** — [basecamp.com/shapeup](https://basecamp.com/shapeup) · persona-adjacent thinking on how user problems get framed before being solved

---

## Licence

This repository is published under [CC-BY-4.0](LICENSE). You can adapt, remix, and build on it freely — including commercially — provided you give appropriate credit.

The personas in this repository are fictional. Any resemblance to real people is coincidental and unintended.
