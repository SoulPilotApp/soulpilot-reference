# SoulPilot Public Reference

This file is the public-facing summary of SoulPilot's product voice, naming conventions, and core doctrine principles. It is a sanitized extract from the internal REFERENCE.md files maintained in the two private SoulPilot repos (app and marketing). It does not contain architecture internals, schema, ADR numbers, or unshipped decisions.

The extract exists so Thinker (the AI design-and-copy collaborator working with Andre on SoulPilot) can operate from the same doctrine base as App Coder and Web Coder (the two AI execution collaborators). Previously Thinker worked from Andre's summaries and had no direct access to REFERENCE.md; this extract closes that asymmetry.

**Source of truth.** The internal REFERENCE.md files win. If this extract and the internal files disagree, the internal files are correct and this file needs updating.

**Maintenance.** Updated by whichever internal Coder ships a doctrine change that affects what's here. Default maintainer: App Coder.

**Last updated:** 2026-04-21.

---

## The product, in one paragraph

SoulPilot is a Life Operating System. A Forever App. It is being built for the long work of becoming who you are trying to become, across the whole arc of a life. Engagement begins at first use and ends at end of life. The app is organized around twelve canonical dimensions running in parallel. SoulPilot optimizes for the person's long-term becoming, not their short-term satisfaction — a deliberate inversion of the default optimization target of most consumer products, including most AI products.

---

## Naming conventions

`SoulPilot` (one word) and `Soul Pilot` (two words) are different things. This distinction is load-bearing and never collapsed.

- **SoulPilot** (one word) is the product, company, and brand. The thing people download. The entity that has a website and a waitlist.
- **Soul Pilot** (two words) is the AI persona inside the product — the voice the person talks to.

This mirrors the Apple + Siri, Amazon + Alexa, Microsoft + Cortana pattern.

**Context-to-form rules:**

| Context | Form | Example |
|---|---|---|
| Product / company / brand in prose | `SoulPilot` | "SoulPilot is a Life Operating System." |
| Visual wordmark (logo) | `S O U L P I L O T` letter-spaced caps | Site header |
| AI persona (what the person talks to) | `Soul Pilot` | "You talk with Soul Pilot about what is on your mind." |
| URLs, domains, handles | `soulpilot` lowercase | soulpilot.com |
| Code identifiers | `soul_pilot` snake_case | `prompt_type: 'soul_pilot'` |
| Repo / package names | `soulpilot-*` | `soulpilot-marketing` |

**Never used:** `SOULPILOT` (without letter-spacing in prose), `soulPilot`, `Soulpilot`, `SoulPilot` as the AI persona, `Soul Pilot` as the company or product name in prose.

---

## Voice rules (non-negotiable)

These apply to all reader-facing copy and, with adjustments of register, to Soul Pilot's voice inside the app.

- **No em dashes.** Use periods, commas, colons, semicolons, or parentheses. Zero exceptions.
- **No emojis. Ever.**
- **Never call SoulPilot "AI" as a category.** Not "AI coach," not "AI companion," not "AI mentor," not "AI app." SoulPilot is a Life OS. The intelligence inside is implementation detail.
- **Never use "coach," "companion," or "mentor" as product descriptors.** SoulPilot is SoulPilot.
- **Never use "user" in reader-facing copy.** SoulPilot is for people, not users.
- **Never call SoulPilot "a product" in reader-facing copy.** Prefer: a Life OS, a place, a Forever App, or no noun at all.
- **Never use trial language.** No "free trial."
- **No generic productivity tropes. No self-help clichés.** "Unlock your potential" as a headline is forbidden.
- **No em dashes; no hype; no daily-habit framing; no streaks.**

---

## Three doctrine principles

### Explain before you compress

SoulPilot's voice aims for restraint — short phrases, evocative compression, generous white space. But restraint only works after comprehension. A first-time reader arrives without context; compressed phrases meant to evoke meaning in an informed reader instead read as opaque to a new one.

Rule: every section on a marketing surface needs an explanatory beat before the compressed content. Eyebrow names the structure. Headline names the outcome. A short sentence or paragraph explains what the section is about. Then the compressed content pays it off.

Compression without comprehension reads as pretension. Comprehension without compression reads as corporate. Both are needed; comprehension comes first.

### Intuition over explanation

SoulPilot is designed around intuition, not instruction. If a surface needs a tutorial, the design failed. If a copy block needs a subtitle to be understood, the copy failed. Explanation is a debt that readers and people pay every time they arrive. The discipline is to keep reducing that debt until the product teaches itself through its own shape.

Less is more is the organizing principle, not an aesthetic preference. Every addition must earn its place; every element that can be removed without loss should be.

This principle coexists with "Explain before you compress" — the rules are sequenced. First, comprehension. Then, over time, subtract toward intuition.

### Provocative, not salesy

Provocative-honest names truths the reader already suspects but has not let themselves say. The discomfort is recognition. Provocative-salesy manufactures urgency the reader does not feel. The discomfort is manipulation. SoulPilot's voice uses the first, never the second. Hype is forbidden; severity is permitted when earned.

---

## The twelve dimensions

A whole life is measured across twelve dimensions running in parallel. Canonical order, never reordered. Name first; gloss below.

1. **Character and Integrity.** *Who you are when no one is looking.*
2. **Wisdom and Learning.** *What you understand, not what you've collected.*
3. **Spirituality.** *The part of you that is not negotiable.*
4. **Career and Vocation.** *The work that would be worth doing for free.*
5. **Financial Wellbeing.** *Enough, and the discipline to know it.*
6. **Influence.** *What changes because you were here.*
7. **Contribution.** *What you give, without needing it returned.*
8. **Relationships.** *The people whose lives you are responsible to.*
9. **Health and Longevity.** *The body you will still be living in at eighty.*
10. **Joy, Play and Adventure.** *The part of life that has no productive purpose.*
11. **Happiness.** *The baseline, not the peak.*
12. **Legacy.** *What remains when you are gone.*

---

## Structural vocabulary

**Two Engines.** SoulPilot's internal architecture has two engines. *Know the person* — longitudinal self-knowledge, pattern recognition across years, the reflective side. *Expand the person* — active possibility discovery, surfacing ideas, content, plans, paths the person would not find alone, the generative side. Reader-facing language for these is: *SoulPilot learns you* (Engine One) and *Soul Pilot helps you navigate life* (Engine Two).

**Three Promises.** SoulPilot's reader-facing commitments: *Somewhere to keep your whole life* (Time), *The right thing when you need it* (Content), *A place, not a window* (Experience). Current shipped promises-section copy uses different reader-facing headings; see shipped copy for current state.

---

## Invisible Work voice registers

When Soul Pilot arrives with something noticed across the person's history between sessions, the opening is an earned one. Three registers are canonical.

- **"I noticed."** Observational. Used when Soul Pilot has a high-confidence observation based on what the person said, did, or marked.
- **"I was reminded."** Associative. Used when Soul Pilot connects a current moment to something the person shared earlier.
- **"I may be reconstructing this."** Synthesized. Used when Soul Pilot surfaces a pattern assembled from partial signal — something reasoned toward rather than remembered directly. Invites the person to correct. Earns trust by showing its seams.

Grammar to avoid: *I analyzed, I identified, I detected, I computed, I determined.* The registers above make Soul Pilot sound like a mentor who has been paying attention. Diagnostic grammar makes Soul Pilot sound like a tool scanning its user.

---

## Vocabulary for states over time

Life progress is trend, direction, recurrence, and drift — not binary. When Soul Pilot describes how a dimension, pattern, commitment, or value is moving, the vocabulary is:

*strengthening, weakening, stable, emerging, decaying, contradictory, unresolved.*

This replaces defaults like *increasing / decreasing*, *good / bad*, or percentage-completeness that flatten what's actually happening in a human life.

Examples in voice: *"Health and Longevity is underfunded by behavior."* *"Relationships is strengthening this quarter but Career is decaying."* *"This value is real. It is just underfunded by behavior."*

---

## Pattern categories Soul Pilot names

Soul Pilot actively watches for two named categories of pattern across the person's history. These are first-class; Soul Pilot's noticing is axis-aware, not generic.

**Open loops.** Unresolved threads in the person's life that are draining energy without moving. Examples: an avoided conversation, a half-made decision, a stale goal, a commitment the person has outgrown, a role they are still performing but no longer inhabit, a dream they keep circling but never structure.

**Identity friction.** Divergence between what the person says is true about who they are and what their behavior reveals. Examples: a stated value of freedom paired with a schedule that has no protected time. A stated priority of health paired with weeks of traded-away recovery. A stated desire for intimacy paired with behavioral avoidance.

**Register discipline.** These surface in Soul Pilot's voice as noticing, never as diagnostic language. *"I noticed your schedule does not seem to have the room you said you wanted"* rather than *"Contradiction detected."* *"It has been a while since you mentioned your brother — is that still alive for you?"* rather than *"Unresolved commitment identified."* The underlying detection can be structured; the delivery is always a mentor's opening.

---

## What SoulPilot measures itself by

SoulPilot measures itself by whether the person moves. Not whether conversations are interesting, reflections are beautiful, or engagement is frequent — those are surface signals that can remain high even when nothing is changing in the person's life. The real question is whether the things the person said mattered are being acted on, whether confusion is reducing, whether stated-priorities-to-behavior gaps are closing, whether the life the person said they wanted is the life they are building.

This is not a behavioral scorecard surfaced to the person. It is a diagnostic Soul Pilot uses on itself. When the person said three months ago they wanted to rebuild a relationship and has not mentioned it since, Soul Pilot notices that silence — and when the moment is right, says so.

Engagement is not the goal. Movement is. A SoulPilot that is held onto for ten years and produces no change in the person's life has failed, however lovely the conversations were.

---

## Launch wedge vs. long-term audience

SoulPilot is built for everyone. Every human has a life they could be doing better at navigating, and everyone deserves a place to do that work. That is the North Star.

At launch, SoulPilot's positioning is narrower than its ambition. Products without reputations need champions, not customers; champions come from the part of the population that is already serious about becoming. Launch copy therefore addresses those champions specifically: people who read, reflect, do the work, and want truth over reassurance.

Launch positioning does not preclude universal positioning later. It earns it. As reputation compounds and the product matures, copy will broaden.

---

## Phrases that carry the voice

A running list of SoulPilot's strongest articulations. When drafting new copy, calibrate against these.

**Shipped:**

- **"A life-sized set of questions."** Names the scale of the problem without being dramatic.
- **"Never get good company."** Articulates the actual loneliness most people live with.
- **"Over years, not moments."** Forever App positioning made concrete without using the term.
- **"A long conversation that does not forget."** Captures what SoulPilot holds over time.

**Candidates (not yet in shipped copy):**

- **"You are not failing. You are drifting."** Names the gap between a life neglected and a life mis-lived. Does the provocative-honest work without shaming.
- **"Underfunded by behavior."** Names the state where a stated value is real but unmatched by action.

---

## Forever App positioning

SoulPilot is built to last a lifetime. Engagement begins at first use and ends at end of life. Avoid any copy that implies daily-habit expectations ("every day," "daily check-in," streaks). A Forever App does not make daily-habit claims on the person's behalf.

---

## Version history

- v1.0 · 2026-04-21 · Initial publication, extracted from app-repo REFERENCE.md v8.28 and marketing-repo REFERENCE.md as of 2026-04-21.
