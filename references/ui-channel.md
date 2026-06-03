# UI Copy Channel Guide

Use this reference when writing tooltips, empty states, error messages, onboarding copy, button labels, notifications, confirmation dialogs, or any in-product text that lives as a static label in the interface.

This channel is distinct from `micro-channel`. UI copy is authored once and stays put. Micro copy is generated for a specific moment, often per request, often paired with live data. Different intent, related craft.

## Where the voice lives

This file describes the shape of UI copy, not how each archetype sounds in UI form. For archetype voice (tone, rhythm, sentence patterns, vocabulary, anti-patterns), read the archetype file at `references/archetypes/<name>.md`. The Sentence Patterns and Language Domain sections there are the canonical voice references; apply them within the channel rules below.

## Core principle

UI copy is read in the middle of doing something. It should help the user continue, not stop them to read. Every word earns its place or gets cut.

## Workflow

For UI copy, write directly and show 2-3 options per piece. No edit plan needed. The author picks or mixes.

## Copy types and constraints

### Error messages
- Lead with what happened, then what to do.
- Never blame the user.
- Keep under 2 sentences.
- If the error is recoverable, say how.

### Empty states
- Acknowledge the emptiness briefly.
- Explain what will appear and when.
- Optionally suggest an action to get started.
- Keep under 2 sentences.

### Tooltips
- One sentence, ideally under 15 words.
- Define the concept, not the UI element.
- No "Click here to..." (the user can see the button).

### Button labels
- 2-4 words.
- Use verbs that match the action ("Start pilot", "View report", "Export data").
- Match the action, not the destination.

### Onboarding copy
- One idea per step.
- Show progress (step 2 of 4).
- Focus on what the user gains, not what the system does.

### Confirmation dialogs
- State what will happen in plain terms.
- If destructive, name what is at risk.
- Primary action label matches the consequence ("Delete team", not "OK").

### Notifications
- Lead with the change or event.
- Keep under 1 sentence.
- Link to details rather than explaining inline.

## Output format

Present options like this:

```
**[Copy type and brief subject]**

Option A:
"[Label or sentence in the chosen archetype voice, channel-compliant.]"

Option B:
"[Different phrasing or sentence pattern, same archetype.]"

Option C:
"[A third variant for the author to pick from.]"
```

## Quality checks

- [ ] Under the word limit for the copy type.
- [ ] Archetype voice is recognisable but not performed (verified against the archetype's Sentence Patterns and Language Domain).
- [ ] Actionable: the user knows what to do next when applicable.
- [ ] No jargon the user would not know.
- [ ] No blame or condescension in error states.
- [ ] Read aloud: sounds like a person, not a system.
