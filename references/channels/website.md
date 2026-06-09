# Website Channel Guide

Use this reference when writing or editing website pages, landing pages, or long-form marketing content.

## Target metrics

| Metric | Draft | After editing |
|--------|-------|---------------|
| Length | 100% | 40-60% |
| Sections | 12-15 | 5-7 |
| Rhythm | Uniform | Varied |
| Opening | Explanation | Tension |

## Workflow

1. Receive draft (or write one internally if starting from scratch)
2. Perform Core Teaching Analysis (required, see below)
3. Propose edit plan
4. Wait for human approval
5. Execute approved edits

If foundation docs define page structure, narrative arc, or perspective, follow those constraints and apply craft principles within them.

## Core Teaching Analysis

This step prevents duplicate sections, which is the most common problem in drafts.

**Step 1: List each section.** For each section, write the section title and its core teaching in one sentence: what is the single thing this section teaches?

**Step 2: Identify duplicates.** Group sections with the same core teaching, even if they use different formats. A table showing "reading builds vocabulary over time" and a scenario showing the same thing teach the same thing. Both are redundant. Keep only the more engaging one.

**Step 3: Select survivors.** For each group of duplicates, pick the most engaging format. Merge or cut the rest.

Example:
```
Section: "How it works" (feature list)
Core teaching: The app learns your reading pace and adjusts recommendations.

Section: "In practice" (reader scenario)
Core teaching: The app learns your reading pace and adjusts recommendations.

DUPLICATE: Same teaching, different format.
DECISION: Keep the scenario (more engaging), cut the feature list.
```

## Section-by-section guidance

**Hero / Opening:** The draft pattern is to explain what it is. Your job: create tension about the problem it solves.
- Before: "This app gives readers a smarter way to discover books, using reading history and preferences to surface titles they'll actually finish."
- After: "Most reading lists grow. Most books on them never get opened."

The hero line is a headline. Write it last, after the rest of the page exists, so it can point at the sharpest thing the page earned. See `references/channels/headline.md`.

**Middle sections:** Keep 3-4 sections that build tension toward insight. Cut the rest. For each section ask: Does this move the reader forward or just inform them? Could this live on a linked page?

**Closing:** End with momentum, not summary.
- Before: "Readers who use the app consistently report finding more books they enjoy and spending less time browsing."
- After: "Your next favourite book is already in the catalogue. Find it."

## The Defer move

Depth lives on linked pages, not inline.

Instead of three paragraphs explaining how the recommendation engine works, write one sentence with a link:
"The more you read, the sharper your recommendations get. [See how the engine works](/features/recommendations)"

## Related links

Every page exists in a journey. After reading, where should the reader go?

For each link, specify:
- **Link text** (action-oriented, curiosity-inducing)
- **Target page**
- **Intent** (why relevant from this page)
- **Coverage** (what the linked page should cover)

Link types to consider:
- Depth links: detailed explanation of something mentioned briefly
- Lateral links: related concept the reader might also care about
- Persona links: "If you're a [role], see [page]"
- Action links: next step in the journey

## Calls to action

Propose a primary CTA (the main action) and a secondary CTA (lower commitment).

Good CTAs are specific:
- Bad: "Learn more"
- Good: "Browse your first personalised shelf"
- Good: "Talk to someone who's done this"

Match CTA to page intent:
- Awareness (what is this?) -> "See how it works" / "Read a case study"
- Consideration (is this for me?) -> "Talk to us" / "See pricing"
- Validation (prove it) -> "Try it free for 30 days" / "Read the reviews"

## Edit plan format

Present this to the user before executing:

```markdown
## Core Teaching Analysis

| Section | Core Teaching |
|---------|---------------|
| [Title] | [One sentence] |

**Duplicates identified:** [Which sections teach the same thing]

## Edit Plan

### CUT
- [Section] - [reason]

### COMPRESS
- [Section]: [current words] -> [target]

### HOOK
Current opening: "[quote]"
Options:
1. "[tension alternative 1]"
2. "[tension alternative 2]"

### VARY
- [Rhythm changes]

### EDGE
Candidates:
1. "[provocative true statement]"

### DEFER
- [Detail] -> link to [page]

### LINKS
| Link Text | Target | Intent | Coverage |
|-----------|--------|--------|----------|

### CTA
**Primary:** "[text]" -> [destination]
**Secondary:** "[text]" -> [destination]
**Placement:** [where]

## Projected Result
- Sections: [X] -> [Y]
- Estimated reduction: [X]%
```

## Editing checklist

- [ ] Core Teaching Analysis completed
- [ ] No duplicate sections remain
- [ ] Length: 40-60% of original
- [ ] Sections: 5-7 maximum
- [ ] Opening creates tension, doesn't explain
- [ ] At least one short punchy section (under 30 words)
- [ ] At least one provocative true statement visible
- [ ] Detailed explanations deferred to linked pages
- [ ] Related links proposed with intent and coverage
- [ ] Primary and secondary CTAs proposed
- [ ] Not telegram-style: sentences flow into each other
- [ ] Read aloud: has energy AND sounds like natural speech

## Common mistakes

- **Over-cutting:** Don't cut concrete examples. Cut the explanations around them.
- **Losing accuracy:** Editing for energy never sacrifices truth.
- **Adding hype:** Edge is not hype. "If you're not ready to hear uncomfortable truths" has edge. "Revolutionary AI platform" is hype.
- **Uniform shortening:** Don't shorten everything equally. Create contrast: some sections short, some longer.

## When to stop editing

**You're done when:** Every section earns its place, the opening creates a question, reading aloud feels energetic not dutiful, a smart skeptic would keep reading.

**You've gone too far when:** Key information is missing, the page feels cryptic instead of intriguing, accuracy has been sacrificed for punch.
