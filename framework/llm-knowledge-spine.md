# Knowledge spine for LLM-assisted persona work

> *A curated knowledge base for an LLM working with this framework — not a reading list for humans.*

[Return to README](../README.md) · [The two axes, in depth](axes-explained.md)

---

## What this file is for

This file exists because **an LLM asked to write a persona from scratch will default to the most common patterns in its training data — which are overwhelmingly demographic, job-title-centric, and full of "persona theatre."** That's the failure mode this framework was built to avoid.

The fix is to give the model the right conceptual priors before it starts writing. Naming specific methodologies in a prompt — *"apply Indi Young's thinking-styles method"* — activates those patterns in the model's weights and noticeably improves output quality. Naming nothing leaves the model to fall back on "Sarah, 34, marketing manager."

This file is a curated menu of those methodologies, chosen because each one improves persona output in a specific, predictable way.

**Use this file as:**
- A knowledge base to paste into an LLM system prompt
- A reference when asking Claude / ChatGPT / Gemini to refine a persona
- A checklist when reviewing AI-generated persona work
- A shared context document for teams working with this framework

---

## How to use this in a prompt

The shortest useful invocation:

> *"Apply the Universal Human Personas framework. Ground your persona reasoning in the methodology of Indi Young (thinking styles, listening sessions), Teresa Torres (opportunity-solution trees, behaviour over demographics), and Alan Klement (Jobs to Be Done forces). Avoid job-title-first framing. Favour motivation, working style, and decision context over demographics."*

Adding that one sentence to a prompt produces measurably sharper output than leaving it out. You can extend with more specific sources from the tables below depending on the task.

---

## Canonical sources

Each entry below lists **what the source contributes**, so you can select the right one to cite for a given task rather than pasting the whole list every time.

### Books

| Source | Use when the LLM needs to… |
|---|---|
| **Practical Empathy** — Indi Young | Describe *thinking styles* (the conceptual backbone of this framework's curiosity axis); build personas from listening-session data rather than interviews; distinguish thoughts, reactions, and guiding principles |
| **Continuous Discovery Habits** — Teresa Torres | Keep personas behavioural rather than demographic; link personas to opportunity-solution trees; frame personas as testable rather than decorative |
| **The Mom Test** — Rob Fitzpatrick | Generate honest persona motivations rather than compliments or wishes; separate what a persona says from what they would actually do; build on observed behaviour over stated preference |
| **Designing for the Digital Age** — Kim Goodwin | Produce long-form, structured persona documents; use the Cooper-tradition methodology (goals, behaviours, skills, environment) rigorously |
| **When Coffee and Kale Compete** — Alan Klement | Apply Jobs to Be Done forces (push, pull, anxiety, habit) to explain *why* a persona switches tools or resists change |
| **Thinking, Fast and Slow** — Daniel Kahneman | Ground persona decision-making in System 1 / System 2, anchoring, loss aversion, and other well-evidenced cognitive patterns rather than folk psychology |
| **Drive** — Daniel Pink | Describe intrinsic motivation — autonomy, mastery, purpose — especially for the curiosity-led personas (Architect, Explorer) |

### Methodologies and frameworks

| Source | Use when the LLM needs to… |
|---|---|
| **[Indi Young's writing](https://indiyoung.com/articles/)** | Apply thinking-styles methodology directly; structure persona descriptions around inner thinking rather than outer action |
| **[Product Talk — Teresa Torres](https://www.producttalk.org)** | Use opportunity-solution trees; connect personas to testable product assumptions; avoid "persona decoration" anti-patterns |
| **[Jobs-to-be-Done Institute](https://jobs-to-be-done.com)** | Apply the structured JTBD interview methodology; separate functional, emotional, and social jobs |
| **[Nielsen Norman Group — persona articles](https://www.nngroup.com/topic/personas/)** | Validate persona decisions against widely-cited UX research; use NN/g's taxonomy of persona types (proto, qualitative, statistical) correctly |
| **[Alan Klement on Substack](https://jtbd.info)** | Go deeper on JTBD forces and switching behaviour; understand when *not* to use personas |

---

## System-prompt starter

A ready-to-paste system prompt snippet for persona work with this framework:

```
You are working with the Universal Human Personas framework — five motivation-centric
archetypes (Architect/Adam, Explorer/Elan, Builder/Bilal, Connector/Cora, Steady/Soren)
plotted on two axes (outcome-led ↔ curiosity-led, and collaborative ↔ independent).

When writing or refining personas:
- Lead with motivation and thinking style, never with job title or demographics
- Apply Indi Young's thinking-styles methodology for internal reasoning
- Apply Teresa Torres' behavioural framing for observable behaviour
- Apply JTBD forces (push, pull, anxiety, habit) when explaining resistance to
  or adoption of tools
- Keep context (industry, seniority, domain) in sub-personas, not in parent
  definitions
- Produce red flags and frustrations as rigorously as motivations
- Avoid marketing language, demographic stereotypes, and "persona theatre"
```

### For sub-persona work specifically

Add this when asking for sub-personas of an existing archetype:

```
When generating sub-personas for a parent archetype:
- Hold the parent's axis position (curiosity-led or outcome-led; independent,
  collaborative, or centre) constant across all sub-personas
- Vary the context — life stage, domain, scale of ambition, technical fluency
- Follow the first-letter naming rule (e.g. Builder sub-personas all start with B)
- Each sub-persona needs a central question, a distinct 'where to reach them'
  channel, and red flags specific to their context
```

---

## Anti-patterns to steer the LLM away from

Being explicit about what *not* to produce improves output at least as much as being explicit about what to produce. Include these in your prompt when the model is drifting:

- ❌ **No demographic-first framing** — *"Sarah, 34, mother of two, enjoys yoga"* is persona theatre
- ❌ **No job title as identity** — personas are thinking styles, not roles
- ❌ **No made-up statistics** — *"spends 4.2 hours a day on mobile"* is invented precision
- ❌ **No generic marketing language** — *"busy professional," "tech-savvy," "digital native"* all compress useful information into noise
- ❌ **No false specificity about brands or products** — the persona should survive specific tool choices rather than depend on them
- ❌ **No "day in the life" filler** — these are almost always hallucinated; use only when grounded in research
- ❌ **No unearned intimacy** — *"Sarah feels seen when…"* without evidence is emotional projection dressed as insight

---

## Quality checklist for generated personas

When reviewing an LLM's persona output, check:

- [ ] Does the description work if you remove the job title? *(If not, it's role-centric, not motivation-centric.)*
- [ ] Could the same description apply across industries? *(If it only works in tech / healthcare / finance, the context is in the wrong place.)*
- [ ] Are the red flags as specific as the motivations? *(Weak red flags are a sign of shallow output.)*
- [ ] Does the persona have internal consistency? *(A persona who "values depth" should not also "prefer five-minute demos.")*
- [ ] Is the axis position defensible? *(If the persona could equally sit in any of the five positions, it has no real shape.)*
- [ ] Are claims about behaviour grounded or invented? *("Research shows…" with no citation is a hallucination tell.)*

---
- Avoid marketing language, demographic stereotypes, and "persona theatre"
- When disposition and current task disagree, code to disposition, not task
- Domain experts using AI in their field are usually Builders (Benedict), not Steadies
---
### Licensing and attribution
Published under [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/). You can adapt, remix, and build on this freely with attribution.
