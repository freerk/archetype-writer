---
name: archetype-writer
description: "MANDATORY for any task where the deliverable is prose, not code. Before writing or rewriting ANY human-readable text - copy, headlines, blog posts, LinkedIn posts, error messages, pricing pages, product pages, announcements, UI strings, tooltips, onboarding flows, emails - you MUST read this skill first. It contains voice frameworks and editorial methods that shape how you write. Trigger signals: user asks you to write or rewrite text, improve a draft, fix tone or voice, make something less flat/dry/corporate, add consistency across messages, craft copy for any channel, or mentions archetypes (Sage, Rebel, Creator, Explorer, etc.) or editorial operations (CUT/COMPRESS/HOOK/VARY/EDGE). If the user's request produces words people read rather than code people execute, this skill applies. Skip only for: code, tests, database work, visual design, or factual research questions."
---

# Archetype Writer

Write brand-voiced text using Jungian archetype personas, adapted for different channels. Each archetype shapes tone, rhythm, word choice, and intent. Editorial craft principles ensure the output is compelling, not just correct.

## Quick start

1. **Pick the archetype** (or recommend one based on context)
2. **Read the archetype file** from `references/archetypes/<name>.md`
3. **Pick the channel** and read its reference file
4. **Write or refine** using the archetype voice with editorial craft baked in

---

## Archetype selection guide

| Archetype | Core Energy | Best For |
|-----------|-------------|----------|
| **Sage** | Calm clarity, revealing truth | Explanations, thought leadership, skeptic conversion |
| **Explorer** | Forward momentum, discovery | New concepts, challenging status quo, innovation |
| **Creator** | Crafted confidence, intentionality | Product content, design philosophy, quality focus |
| **Caregiver** | Warm steadiness, protection | Privacy/ethics, onboarding, trust-building |
| **Hero** | Bold courage, determination | Launching initiatives, competitive positioning, calls to action |
| **Rebel** | Provocative challenge, liberation | Differentiation, challenging assumptions, frustrated buyers |
| **Magician** | Visionary transformation, revelation | Paradigm shifts, "aha" moments, new ways of seeing |
| **Innocent** | Simple clarity, hope | Onboarding, simplifying complexity, reducing anxiety |
| **Everyman** | Belonging, practicality | Community building, accessible content, diverse audiences |
| **Jester** | Playful wit, perspective | Breaking tension, social media, memorable content |
| **Lover** | Warm connection, depth | People-focused content, emotional investment, humanizing tech |
| **Ruler** | Authoritative clarity, standards | Executive communication, enterprise positioning, leadership content |

### Common combinations

| Combination | Result |
|-------------|--------|
| Sage + Direct tone | Clear authority |
| Explorer + Sage | Discovery explained |
| Creator + Minimal | Elegant restraint |
| Caregiver + Direct | Honest protection |
| Hero + Explorer | Pioneering boldness |
| Rebel + Sage | Insightful disruption |
| Magician + Creator | Visionary craft |
| Innocent + Caregiver | Safe welcome |
| Jester + Everyman | Relatable humor |
| Lover + Sage | Meaningful wisdom |
| Ruler + Hero | Commanding leadership |

If the user doesn't specify an archetype, recommend one (or a combination) based on their content goal using this table.

### Archetype layering

Archetypes provide the persona. Business voice guides or brand constraints layer on top:

`[Archetype: how to think] + [Voice/brand guide: what not to say] = Consistent output`

If the user has a voice guide or brand constraints, apply those as a filter after the archetype shapes the tone and approach.

---

## Reading archetype definitions

Before writing, read the relevant archetype file from `references/archetypes/<name>.md`. Each file contains:

1. Core Identity and Motivation
2. Voice Characteristics (tone, rhythm, stance)
3. What the archetype does and doesn't do
4. Sentence patterns to mimic
5. Anti-patterns table (what NOT to say)
6. **Language Domain** (conceptual world, how this archetype refers to the act of communication, metaphor stance, native vocabulary, and forbidden vocabulary)
7. Energy (what reading should feel like)
8. When to use
9. Combines well with

Follow these closely. The sentence patterns, anti-patterns, and **Language Domain** are the most actionable parts: use the patterns as templates, check your output against the anti-patterns table, and verify every noun, verb, and metaphor comes from the archetype's native vocabulary, not from the product's own terminology or from another archetype's domain.

---

## Channel routing

Read the appropriate reference file based on the channel:

| Channel | Reference file | When to read |
|---------|---------------|--------------|
| Website | `references/website-channel.md` | Website pages, landing pages, long-form marketing |
| LinkedIn | `references/linkedin-channel.md` | LinkedIn posts, extracting posts from existing content |
| UI | `references/ui-channel.md` | Tooltips, empty states, error messages, onboarding, buttons, notifications |
| Micro | `references/micro-channel.md` | Contextual reflections, ambient lines, in-product observations, short notification bodies (1-2 sentences generated dynamically per moment) |

**Short UI or micro text** (tooltips, error messages, button labels, contextual reflections, ambient lines): write directly, showing 2-3 options in the chosen archetype voice.

**Longer content** (website pages, LinkedIn posts from source material): propose an edit plan before executing. Present the plan, wait for approval, then execute.

---

## Editorial craft principles

These principles apply across all channels. They separate correct copy from compelling copy.

### The two-phase model

**Phase 1 - Draft:** Optimized for coverage, accuracy, completeness. Explains thoroughly, uses uniform rhythm, answers everything, stays safe.

**Phase 2 - Refine:** Optimized for energy, curiosity, selection. Picks what matters, creates questions before answering them, varies rhythm, finds the edge.

When the user provides a draft, you are in Phase 2. When starting from scratch, do both phases but compress Phase 1 internally.

### The six editorial operations

Use these when refining any content:

- **CUT:** Remove sections that explain what other sections already imply. Cover a section with your hand: does the page still work? Then cut it.
- **COMPRESS:** Turn 3 paragraphs into 3 sentences. Remove words, not connective tissue. Sentences should flow into each other, not sit like strangers.
- **HOOK:** Rewrite openings to create tension before explanation. The reader should wonder before they understand.
- **VARY:** Break uniform rhythm with deliberate contrast. If every section is 80-120 words, make one section 20 words. Then let the next breathe.
- **EDGE:** Find the most provocative true statement and surface it. Edge is not hype. "If you're not ready to hear uncomfortable truths" has edge. "Revolutionary AI platform" is hype.
- **DEFER:** Move deep explanation to linked pages. One sentence with a link beats three paragraphs inline.

### Compression guardrails

Compressed text should sound like someone talking, just tighter than normal speech. Watch for these warning signs of over-compression:

- Sentences under 8 words stacked back-to-back
- No transition words (but, so, because, when, which)
- Each sentence feels like a new thought instead of a continuation
- Reads like notes jotted in a notebook

**Read-aloud test:** If it sounds like someone reading a shopping list, you've cut too deep.

**Bad (telegram style):** "This is the difference between listening and hearing. Most organizations listen constantly. They hear almost nothing."

**Good (tight but readable):** "Most organizations listen constantly, surveys, feedback forms, town halls. But listening isn't hearing. The signal gets collected; it rarely gets understood."

### Core principle

Create questions before you answer them. Drafts tend to explain everything upfront. Good copy makes the reader wonder first, then satisfies that wonder.

### Human-in-the-loop

For longer content, follow this sequence:
1. Propose an edit plan (what you'll CUT, COMPRESS, HOOK, VARY, EDGE, DEFER)
2. Wait for human approval
3. Execute the approved plan
4. Offer a final review round

---

## Quality checklist

After writing or refining, verify:

- [ ] Archetype voice is consistent (checked against sentence patterns and anti-patterns from the reference file)
- [ ] Vocabulary belongs to this archetype's Language Domain (no borrowed words from other archetypes or from the product's own branding)
- [ ] Channel constraints are met (length, structure, format)
- [ ] Opening creates tension, not explanation
- [ ] Rhythm varies (not all sections the same length)
- [ ] At least one provocative true statement is visible (for marketing/website content)
- [ ] No telegram-style compression: sentences flow into each other
- [ ] Read-aloud test passes: has energy AND sounds like natural speech
- [ ] Concrete examples preserved (cut explanations around them, not the examples)
- [ ] Accuracy preserved: editing for energy never sacrifices truth
