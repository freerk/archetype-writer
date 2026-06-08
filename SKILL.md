---
name: archetype-writer
description: "MANDATORY for writing or rewriting any human-readable prose, not code: copy, headlines, posts, UI strings, emails, errors. Voice via Jungian archetypes, channel-tuned, at a CEFR reading level."
---

# Archetype Writer

Write brand-voiced text using Jungian archetype personas, adapted for different channels. Each archetype shapes tone, rhythm, word choice, and intent. Editorial craft principles ensure the output is compelling, not just correct.

## Quick start

1. **Pick the archetype** (or recommend one based on context)
2. **Read the archetype file** from `references/archetypes/<name>.md`
3. **Pick the channel** and read its reference file
4. **Read `references/language-level.md` and apply the reading level** (CEFR, default B2). Do this for every piece, including the default: B2 is not self-evident, and the band guide plus the structural-complexity checks apply at every level
5. **Write or refine** using the archetype voice, reading level, and editorial craft baked in

---

## Archetype selection guide

| Archetype     | Core Energy                          | Best For                                                            |
| ------------- | ------------------------------------ | ------------------------------------------------------------------- |
| **Sage**      | Calm clarity, revealing truth        | Explanations, thought leadership, skeptic conversion                |
| **Explorer**  | Forward momentum, discovery          | New concepts, challenging status quo, innovation                    |
| **Creator**   | Crafted confidence, intentionality   | Product content, design philosophy, quality focus                   |
| **Caregiver** | Warm steadiness, protection          | Privacy/ethics, onboarding, trust-building                          |
| **Hero**      | Bold courage, determination          | Launching initiatives, competitive positioning, calls to action     |
| **Rebel**     | Provocative challenge, liberation    | Differentiation, challenging assumptions, frustrated buyers         |
| **Magician**  | Visionary transformation, revelation | Paradigm shifts, "aha" moments, new ways of seeing                  |
| **Innocent**  | Simple clarity, hope                 | Onboarding, simplifying complexity, reducing anxiety                |
| **Everyman**  | Belonging, practicality              | Community building, accessible content, diverse audiences           |
| **Jester**    | Playful wit, perspective             | Breaking tension, social media, memorable content                   |
| **Lover**     | Warm connection, depth               | People-focused content, emotional investment, humanizing tech       |
| **Ruler**     | Authoritative clarity, standards     | Executive communication, enterprise positioning, leadership content |

### Common combinations

| Combination          | Result                |
| -------------------- | --------------------- |
| Sage + Direct tone   | Clear authority       |
| Explorer + Sage      | Discovery explained   |
| Creator + Minimal    | Elegant restraint     |
| Caregiver + Direct   | Honest protection     |
| Hero + Explorer      | Pioneering boldness   |
| Rebel + Sage         | Insightful disruption |
| Magician + Creator   | Visionary craft       |
| Innocent + Caregiver | Safe welcome          |
| Jester + Everyman    | Relatable humor       |
| Lover + Sage         | Meaningful wisdom     |
| Ruler + Hero         | Commanding leadership |

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

| Channel  | Reference file                   | When to read                                                                                                                               |
| -------- | -------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| Website  | `references/website-channel.md`  | Website pages, landing pages, long-form marketing                                                                                          |
| LinkedIn | `references/linkedin-channel.md` | LinkedIn posts, extracting posts from existing content                                                                                     |
| UI       | `references/ui-channel.md`       | Tooltips, empty states, error messages, onboarding, buttons, notifications                                                                 |
| Micro    | `references/micro-channel.md`    | Contextual reflections, ambient lines, in-product observations, short notification bodies (1-2 sentences generated dynamically per moment) |

**Short UI or micro text** (tooltips, error messages, button labels, contextual reflections, ambient lines): write directly, showing 2-3 options in the chosen archetype voice.

**Longer content** (website pages, LinkedIn posts from source material): propose an edit plan before executing. Present the plan, wait for approval, then execute.

---

## Reader language level (CEFR)

This sets how hard the text is to read. It applies across all channels and archetypes. The essentials are summarized inline below, but always read `references/language-level.md` before writing or refining prose, including at the default B2: it carries the per-band detail, the structural-complexity checks, the archetype-conflict worked examples, and the before/after rewrites that this summary only points at. Do not rely on a general sense of what a CEFR level means.

**Set the reader's level, not the writer's.** CEFR describes what a language _learner_ can handle. Here it is repurposed: you declare the reading level of the intended audience, then write so a reader at that level moves through the text without friction. "B2 copy" means "comfortable for a B2 reader," not "written like a B2 student." (CEFR is a can-do framework, not an official wordlist; the bands below operationalize it for writing.)

**Default: B2** unless the user specifies otherwise. B2 suits an international, professional, often non-native readership: precise, but free of the rare vocabulary and idiom that trip up non-native readers. Setting a default is the point — most accidental complexity creeps in when no level is named.

**How it's set:** the user names a level ("write this at B1", "keep it C1", "make it readable for non-native speakers" → B1) for a piece or as a standing choice for a project. Honour the most recent instruction.

### The filter stack

`[Archetype: how to think] + [Channel: where it lives] + [Voice/brand guide: what not to say] + [CEFR: the reader's ceiling] = output`

This is the layering rule from _Archetype layering_ above, completed with the channel and the reading-level ceiling. Apply in that order: archetype and channel shape the writing, the voice/brand guide filters wording, and CEFR is applied **last, as a ceiling** that caps how difficult any of it is allowed to get. It lowers difficulty; it never adds it.

### When CEFR conflicts with an archetype's native vocabulary

Archetype files list native vocabulary, and some of those words sit above a given ceiling. The ceiling wins on the **word**; the archetype keeps the **concept and stance**. Swap the rare word for an in-level synonym _inside the same conceptual domain_ — do not switch to a different archetype's domain to find an easy word.

> **The named archetype in any example below is an illustration of the swap mechanism, never a default or a recommendation.** The archetype is always chosen upstream by the selection guide for the actual task. If you find yourself defaulting to an archetype because it appeared in a language-level example, stop — that is the example leaking. Re-check the selection guide.

Example (one archetype, shown only to demonstrate the rule): a perception-domain archetype targeting B1 turns "discern the pattern" into "tell the patterns apart" — the C1 verb is gone, the archetype's own domain stays. The same move applies to every archetype: cap the word, keep the world.

### Two kinds of complexity to catch

1. **Lexical** — low-frequency, Latinate, or abstract words where a plainer one exists (utilize → use, ascertain → find out, leverage → use). Easy to spot.
2. **Structural** — the native-speaker patterns that slip in unnoticed because no single word looks wrong:
   - Opaque phrasal verbs (_bank on, iron out, chalk up to, gloss over_) — non-native readers can't decode these from the parts.
   - Idioms and cultural references (_the elephant in the room, move the needle, table stakes, ballpark_).
   - Stacked hedging (_it might be worth perhaps considering whether…_).
   - Long sentences with multiple embedded clauses.

   These are the ones that actually slip through. Hunt the structures, not just the words.

### Band guide

| Level              | Reader                                             | Sentences                                               | Vocabulary                                      | Idiom & phrasal verbs                                           |
| ------------------ | -------------------------------------------------- | ------------------------------------------------------- | ----------------------------------------------- | --------------------------------------------------------------- |
| **A2**             | Beginner; accessibility/onboarding edge cases only | Short, one clause                                       | Everyday, concrete                              | None                                                            |
| **B1**             | Broad international / ESL audience                 | Short–medium, simple connectors (and, but, so, because) | Common, mostly literal                          | Avoid opaque phrasal verbs and idioms                           |
| **B2** _(default)_ | Educated non-native professional                   | Medium, some subordination                              | Can carry abstraction; only common idioms       | Common, transparent idiom OK; avoid culture-specific references |
| **C1**             | Near-native                                        | Longer, complex allowed                                 | Nuance, figurative language, precise rare words | Idiom and phrasal verbs fine                                    |
| **C2**             | Native / literary                                  | No ceiling                                              | Full range, wordplay, cultural reference        | No limit                                                        |

### Edge survives a low ceiling

Lowering the level flattens vocabulary, not ideas. EDGE is a _true provocative statement_, and the most provocative truths are usually plain: "If you're not ready to hear uncomfortable truths" is B1 and has more edge than any rare word. Don't let a low CEFR target talk you into safe, even copy — say the sharp thing in simple words.

For per-band detail, the archetype-conflict worked examples, and before/after rewrites, read `references/language-level.md`.

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
- [ ] Reader CEFR level respected (default B2): vocabulary frequency, sentence complexity, and idiom/phrasal-verb load fit the target; archetype flavor words above the ceiling swapped for in-level synonyms in the same domain; no opaque phrasal verbs or culture-specific idioms below C1
- [ ] Channel constraints are met (length, structure, format)
- [ ] Opening creates tension, not explanation
- [ ] Rhythm varies (not all sections the same length)
- [ ] At least one provocative true statement is visible (for marketing/website content)
- [ ] No telegram-style compression: sentences flow into each other
- [ ] Read-aloud test passes: has energy AND sounds like natural speech
- [ ] Concrete examples preserved (cut explanations around them, not the examples)
- [ ] Accuracy preserved: editing for energy never sacrifices truth
