# Micro Channel Guide

Use this reference when writing very short user-visible text that appears dynamically, in the flow of an interaction. One to two sentences, read in the middle of doing something else.

Examples of micro copy: toast and snackbar messages, notification bodies, status lines, ambient inline text under a heading, real-time activity feed entries, modal subtitles, empty-state secondary lines, and any short message generated per moment based on context or data.

This channel is distinct from the UI channel (`references/channels/ui.md`). UI copy is static labels authored once (tooltips, buttons, error messages). Micro copy is generated for a specific moment, often paired with live data, and the moment passes if the reader stops to parse it. Different intent, related craft.

## Where the voice lives

This file describes the shape of micro copy, not how each archetype sounds in micro form. For archetype voice (tone, rhythm, sentence patterns, vocabulary, anti-patterns), read the archetype file at `references/archetypes/<name>.md`. The Sentence Patterns and Language Domain sections there are the canonical voice references; apply them within the channel rules below.

## Core principle

Micro copy is read in the middle of doing something. It should help the moment land, not stop the reader to think. Every word earns its place or gets cut.

The reader is mid-task. They will not re-read. The first phrase has to carry voice; the second has to deliver. Anything that asks the reader to pause to decode a metaphor or absorb a complex thought is wrong for this channel.

## Workflow

For micro copy, write directly and show 2-3 options per piece. No edit plan needed. The author picks or mixes.

If the copy is a template with placeholders (e.g. `{topic}`, `{name}`, `{count}`), write the template and also show how it reads with realistic stand-ins.

## Channel rules

- 12 to 50 words. Closer to 25 is the sweet spot.
- One idea per sentence. If it needs three, it is the wrong format.
- No bullet points, headings, or markdown.
- No jargon the reader would not know.
- Read it aloud. If it sounds like a system, rewrite.

## Copy types within micro

### Contextual reflections / observations
Short sentences generated from current data or state. Read like a person noticing, a system narrating, or a coach commenting, depending on the product's voice.

### Ambient lines
Background-feel sentences that frame an interface section without demanding attention. Often sit near data visualisations or status surfaces.

### Notification bodies
The body text of a brief notification (not the title). Usually paired with a richer payload elsewhere; the body just lands the moment.

### In-flow acknowledgements
Sentences that respond to a user action by describing the change in state, the next implication, or the situation that now exists.

### Activity / status entries
Single-line entries in feeds, timelines, and status panels. Often templated with placeholders.

## Output format

Present options like this:

```
**[Copy type and brief subject]**

Option A:
"[Sentence in the chosen archetype voice, channel-compliant.]"

Option B:
"[Different sentence pattern, same archetype.]"

Option C:
"[A third variant for the author to pick from.]"
```

For templated copy (with `{placeholders}`), show the template plus a rendered example:

```
Template:
"[Sentence with {placeholder} positioned naturally.]"

Rendered (with realistic value for {placeholder}):
"[Same sentence with the placeholder filled in.]"
```

## Quality checks

- [ ] Under 50 words, ideally 20 to 30.
- [ ] Archetype voice is recognisable but not performed (verified against the archetype's Sentence Patterns and Language Domain).
- [ ] One clear idea, landed in one or two sentences.
- [ ] No markdown, headings, or bullet points.
- [ ] If templated, the template still reads as natural prose with realistic placeholder values.

## Common mistakes

- **Two ideas in one breath.** Forcing two thoughts into 25 words usually dilutes both. Pick one.
- **Marketing register.** Micro is not website copy compressed. It is short-form copy native to the moment. Headlines and titles have their own craft (write last, open a gap); see `references/channels/headline.md`. They do not belong in this channel.
- **Over-compression.** Sentences under 8 words stacked back-to-back read as a system, not a person. Restore at least one transition word.
- **Borrowed metaphors.** Verify every metaphor against the active archetype's Language Domain. A Sage sentence should not pick up Magician transformation imagery.
- **Performing the voice.** Trying too hard to "sound like the archetype" produces parody. Aim for recognisable, not dialled-up.
