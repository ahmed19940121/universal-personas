# The two axes, in depth

> *Two questions do most of the work. Get them right and the personas fall out naturally.*

[Return to README](../README.md) · [LLM knowledge spine](llm-knowledge-spine.md)

---

## What you'll find here

This file goes deeper than the README. It explains:

- Why the framework uses these two questions and not some others
- What each side of each axis actually feels like in practice
- Why one of the five personas — *The Steady* — sits in the middle rather than in a corner
- How to use the axes to make real decisions about products, content, and strategy

If you just want the headline version, [the README covers it](../README.md#the-two-axes) in under two minutes.

---

## First, why build a framework this way at all

Andrej Karpathy has a habit of teaching from first principles. When he explains a transformer, he doesn't hand you the API — he rebuilds the thing from scratch, in public, so you end up with a working mental model rather than a list of facts about it. The lesson generalises: *a real model beats any amount of surface knowledge, because the model generates the answers while the knowledge just lists them.*

Persona work has the same property at its best. A great persona isn't a demographic snapshot or a job-title dossier; it's a model of **how someone thinks**. Given a clean model, you can work out what someone will tolerate, what will frustrate them, and what they'll pay for — without having to memorise a long list of facts about them.

Most persona frameworks don't work this way. They describe users by job title — *"The CTO," "The Frontend Developer," "The Marketing Manager"* — and they stop being useful the moment you step outside the industry they were built for. They also age badly, because job titles drift faster than human motivations do.

This framework takes a different approach. **Five archetypes. Two questions. One rule: context (industry, seniority, domain) lives in sub-personas, never in the parent definitions.** What you end up with is a model you can apply to anyone using any tool.

---

## Why these two questions and not others

Most frameworks pick axes that sound professional but don't actually travel. The two common traps:

**Demographics — age, income, job title, industry.** These age badly. "Millennials" was a useful category ten years ago; today it spans people in their late twenties and people in their mid-forties with wildly different relationships to technology.

**Org-chart position — decision-making power, team size, budget authority.** These only work inside a company. They leave out students, freelancers, solo founders, retired people, volunteers, and the enormous population of people using tools outside any organisational structure at all.

A framework built for modern tools — and especially AI tools — needs axes that work for a university student, a staff engineer, a therapist, a middle manager in the public sector, and a retiree writing better emails to their GP. All of those people might pick up the same tool tomorrow.

So this framework uses two questions that work for everyone, regardless of job, age, or background:

1. **Why did you pick up the tool?** *(outcome-led ↔ curiosity-led)*
2. **How do you like to think?** *(collaborative ↔ independent)*

Both are about how someone *works*, not about where they sit on an org chart. That's the trick that lets the framework travel.

---

## Question 1: Why did you pick up the tool?

```
outcome-led  ←─────────────────────────→  curiosity-led
 "finish it"                              "understand it"
```

Some people reach for a tool because they have a job to do. Others reach for a tool because they want to understand something new. That difference changes almost everything about what they want from the experience.

This is **not a measure of intelligence, experience, or ambition.** An outcome-led user can be a world-class expert who simply values their time. A curiosity-led user can be a total beginner who wants to learn deeply. The question is about what draws them in, not how good they are.

### Signs someone is outcome-led

- Asks *"can it do X?"* rather than *"how does it work?"*
- Skims the documentation looking for the example they can copy
- Sticks with the defaults and moves on
- Gets frustrated when a tool makes them choose before it'll give them anything
- Wants the tool to have strong opinions so they don't have to form their own

### Signs someone is curiosity-led

- Asks *"what's really going on underneath?"*
- Reads the documentation from start to finish, including the philosophy bits
- Customises the defaults before they've even used the tool once
- Gets frustrated when a tool hides what it's doing
- Wants the tool to show its workings so they can form their own opinions

### Why this matters for AI tools

AI tools have a particular challenge here: **the same product often needs to serve both kinds of user.** Outcome-led users want a magic button that just works. Curiosity-led users want to see the prompt, tweak the settings, and understand *why* the model said what it said. A product that only serves one of those audiences leaves half its potential users behind.

---

## Question 2: How do you like to think?

```
              independent
                  ↑
                  │
                  │
                  ↓
             collaborative
```

Some people think best when they're left alone. They want to draft, refine, and polish before showing anyone. Others think best out loud, through back-and-forth — whether that's with a colleague, a coach, or an AI.

This is **not about introvert versus extrovert, or junior versus senior.** Some very senior people do their best thinking in conversation. Some very junior people prefer to work things out alone before they'll say a word. The axis is about how someone's brain likes to process, not about their personality type or their seniority.

### Signs someone is independent

- Drafts first, shares later — rarely shares a half-formed idea
- Uses AI as a reference or a rubber duck, not a thinking partner
- Prefers one long, complete answer they can read whole
- Finds back-and-forth exhausting for anything simple
- Happy to disappear with a tool for an afternoon and re-emerge with something finished

### Signs someone is collaborative

- Thinks in dialogue, often talking to themselves out loud
- Uses AI as a partner — something to bounce ideas off
- Prefers short exchanges with lots of small course-corrections
- Finds a single wall of text harder to process than five short turns
- Wants to be met where they are, not handed a finished document

### Why this matters for AI tools

Chat interfaces are a *gift* to collaborative thinkers. For the first time, they have a thinking partner available at any hour. But the same chat interface can feel like a waste of time to an independent thinker, who wanted a complete answer and got a twenty-turn conversation instead. Good AI tools serve both — by making the same underlying capability available in both a "give me the whole thing" mode and a "let's work through it together" mode.

---

## The five positions

Put the two questions together and you get a map. The five personas live at five different points on that map:

| Persona | Why they pick up the tool | How they like to think | Where they sit |
|---|---|---|---|
| 🟣 **Architect** *Adam* | Curiosity-led | Independent | Top-right |
| 🔵 **Explorer** *Elan* | Curiosity-led | Collaborative | Bottom-right |
| 🟠 **Builder** *Bilal* | Outcome-led | Independent | Top-left |
| 🩷 **Connector** *Cora* | Outcome-led | Collaborative | Bottom-left |
| 🟢 **Steady** *Soren* | Outcome-led | **Middle** | Mid-left |

Four of the five sit at the corners. One — *The Steady* — sits deliberately in the middle.

---

## Why The Steady sits in the middle

This is the question the framework gets asked most often, so it's worth answering properly.

Four personas are at the corners because each of them represents a clear, strong preference. The Architect *really* wants depth and independence. The Connector *really* wants outcomes and collaboration. Strong signal in both directions.

The Steady isn't like that. The Steady is defined by **not wanting to commit to a corner.** They want:

- A proven, safe choice — but not so safe it feels outdated
- Some support and reassurance — but not a hand-holding conversation every step of the way
- A clear recommended path — but not a long tutorial
- Help when things go wrong — but not a community they're expected to join

In other words, The Steady wants the tool to **meet them in the middle.** Not because they're indecisive, but because their defining need *is* to avoid extremes.

And this matters, because **The Steady is the biggest population of the five.** They're the people who adopt a tool after the early adopters have de-risked it. They're the quiet majority who describe themselves with phrases like *"I'm not really a tech person."* They'll stay loyal for years if the tool keeps working — and leave silently, permanently, if it doesn't.

Most persona frameworks miss this population entirely because they're designed around the loud, opinionated, visible users at the corners. A framework without a Steady would be describing a minority and calling it the whole picture.

---

## What the framework deliberately doesn't try to capture

The two axes give you a lot. They don't give you everything. It's worth being honest about the trade-off:

**What the axes do capture:**
- How someone wants to think (alone or out loud)
- What draws them to a tool (a result, or understanding)
- Where they'll feel served or frustrated by a design choice

**What the axes deliberately don't capture:**
- Job title, seniority, or time in the role
- Technical skill level
- Industry or domain expertise
- Age, location, or any other demographic
- Company size

That's not a gap — it's a design choice. The moment you add "senior vs. junior" or "tech vs. non-tech" to a top-level persona framework, the framework stops travelling. It becomes a description of *one slice of one industry* rather than a model of how humans work.

Those missing details don't actually disappear. **They show up in sub-personas.** The Builder archetype has five sub-personas (Bayo, Bilal, Brynn, Benedict, Blake) that all share Builder's outcome-led, independent position but vary by context: student, professional, founder, domain specialist, no-code operator. The same refinement will work for the other four archetypes.

This keeps the top-level model clean and portable. The context lives one layer down, where it belongs.

---

## Using the axes to make decisions

The axes are most useful as a **check against drift.** When you're making a decision about a feature, a piece of content, a marketing campaign, or a sales motion, pause and ask three questions:

1. **Which persona does this serve?** Be specific — pick one.
2. **Which personas does this accidentally exclude?** Equally important.
3. **Is the exclusion deliberate, or did you not notice?**

The third question is where most products quietly go wrong.

It's very easy to end up serving only Architects and Explorers — the loud, curious, online half of the map. Those are the users who show up in early adopter communities, who write reviews, who post on forums. They feel like "the users." But they're a minority of the total audience.

Builders, Connectors, and Steadies are the quieter majority. They're less visible online, less likely to respond to a survey, less likely to post a review. But they're numerically much larger, and they leave silently when a product doesn't serve them. **Most products don't lose them with a dramatic failure — they lose them with a thousand small accidental exclusions.**

The framework is most useful as a tool for catching those exclusions before they ship.
