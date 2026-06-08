# Archetype Writer

Most copy is correct. Very little of it is compelling. The gap between the two is rarely about facts, it is about voice: tone, rhythm, word choice, and the intent underneath the words.

Archetype Writer is a skill for AI assistants that closes that gap. It writes brand-voiced text using twelve Jungian archetype personas, adapts each persona to the channel it lands in, and applies a small set of editorial operations that turn a thorough draft into something worth reading.

It works as a [Claude Code](#use-in-claude-code) skill, in the [Claude.ai app](#use-in-the-claudeai-app), and as [context for ChatGPT](#use-in-chatgpt).

---

## What it is

A persona is a way of thinking, not a costume. Each archetype shapes how the writing observes, what it values, and which words it will and will not use.

- **Twelve archetypes.** Sage, Explorer, Creator, Caregiver, Hero, Rebel, Magician, Innocent, Everyman, Jester, Lover, Ruler. Each one is a full voice definition: core motivation, tone and rhythm, sentence patterns to mimic, anti-patterns to avoid, and a **Language Domain** that fixes the native vocabulary and the words the archetype would never say.
- **Four channels.** Website, LinkedIn, UI microcopy, and Micro (ambient, dynamically generated lines). The same archetype sounds different in a landing page than in an error message, so the channel file sets the constraints.
- **Six editorial operations.** CUT, COMPRESS, HOOK, VARY, EDGE, DEFER. These are what separate copy that is accurate from copy that has energy.
- **Five reading levels (CEFR).** A2 through C2. This sets how hard the finished text is to read, so the same archetype and channel can be tuned for a broad international audience or a near-native one. It is applied as a ceiling on top of everything else: it caps difficulty, it never adds it. The default is B2, and the archetype keeps its voice even when a rare word is swapped for a plainer one.

The model is simple: `[Archetype: how to think] + [Channel: where it goes] + [Editorial craft: how to refine] = consistent, compelling output`, with the reading level capping how hard any of it reads.

### Pick an archetype

| Archetype | Core energy | Best for |
|-----------|-------------|----------|
| **Sage** | Calm clarity, revealing truth | Explanations, thought leadership, skeptic conversion |
| **Explorer** | Forward momentum, discovery | New concepts, challenging the status quo, innovation |
| **Creator** | Crafted confidence, intentionality | Product content, design philosophy, quality focus |
| **Caregiver** | Warm steadiness, protection | Privacy and ethics, onboarding, trust-building |
| **Hero** | Bold courage, determination | Launches, competitive positioning, calls to action |
| **Rebel** | Provocative challenge, liberation | Differentiation, challenging assumptions, frustrated buyers |
| **Magician** | Visionary transformation | Paradigm shifts, "aha" moments, new ways of seeing |
| **Innocent** | Simple clarity, hope | Onboarding, simplifying complexity, reducing anxiety |
| **Everyman** | Belonging, practicality | Community, accessible content, diverse audiences |
| **Jester** | Playful wit, perspective | Breaking tension, social media, memorable content |
| **Lover** | Warm connection, depth | People-focused content, humanizing technology |
| **Ruler** | Authoritative clarity, standards | Executive communication, enterprise positioning |

If you are not sure which one fits, describe the goal and let the assistant recommend one. Archetypes also combine: Sage + Rebel reads as insightful disruption, Creator + Magician as visionary craft.

---

## Use in Claude Code

Claude Code discovers skills automatically from their description, so installation is just placing the folder where it looks.

**For all your projects** (personal skill):

```bash
git clone https://github.com/freerk/archetype-writer.git ~/.claude/skills/archetype-writer
```

**For one project** (shared with your team through the repo):

```bash
git clone https://github.com/freerk/archetype-writer.git .claude/skills/archetype-writer
```

That is the whole setup. From then on, when you ask Claude to write or rewrite prose, it reads `SKILL.md`, then loads the specific archetype and channel files it needs. You do not have to invoke anything by hand. To steer it, name the archetype and channel directly:

> Rewrite this landing page hero in a Sage voice for the website channel.

> Write three error-message variants for an expired session. Caregiver, UI channel.

The skill handles longer content with a human in the loop: it proposes an edit plan (what it will CUT, COMPRESS, HOOK, and so on), waits for your approval, then executes.

---

## Use in the Claude.ai app

The Claude.ai app installs skills as a `.zip`. Download the versioned zip from the latest release:

[**Latest release →**](https://github.com/freerk/archetype-writer/releases/latest)

In Claude.ai, go to Customize → Skills → **+ Create skill**, upload the zip, then enable it. From then on it triggers automatically when you ask Claude to write or rewrite prose, or you can name the archetype and channel directly as in the examples above.

---

## Use in ChatGPT

ChatGPT has no skill system, so you supply the same files as context. There are three ways, from most durable to most ad hoc.

**1. A Project (recommended).** Create a ChatGPT Project, then paste the contents of `SKILL.md` into the project instructions. Upload the archetype files you use most and the channel files from `references/` as project files. Include `references/language-level.md` if you want to set a reading level, since `SKILL.md` points to it for the per-level detail. Every chat in that project then writes with the framework available.

**2. A custom GPT.** Build a GPT, put `SKILL.md` in the instructions, and add the `references/` files as Knowledge. Share it with anyone who needs the same voice.

**3. Paste as context.** For a one-off, paste `SKILL.md` plus the one archetype file and one channel file you need at the top of the chat, then make your request. Add `language-level.md` too if you are targeting a specific reading level. Lighter, but you repeat it each session.

A prompt that works well once the context is loaded:

> Using the Sage archetype and the website channel from the framework above, rewrite the text below. First give me the edit plan, then wait for my go-ahead.

The Language Domain sections matter most here. They are what keep the voice from drifting into generic AI tone, so always include the archetype file you are targeting rather than relying on the name alone.

---

## The method

Good copy is written in two passes. The first pass covers everything: accurate, complete, safe, uniform. The second pass selects: it cuts what other sections already imply, opens with tension instead of explanation, varies the rhythm, and surfaces the one provocative true statement the draft was hiding.

The six operations are the tools for that second pass:

- **CUT** — remove what other sections already imply.
- **COMPRESS** — three paragraphs become three sentences, without losing the connective tissue.
- **HOOK** — open with a question in the reader's mind, not an answer.
- **VARY** — break uniform rhythm with deliberate contrast.
- **EDGE** — find the most provocative true statement and let it show. Edge is not hype.
- **DEFER** — move deep explanation behind a link.

Compression has a limit. Text cut too far reads like a shopping list: short sentences stacked back to back, no transitions, every line a new thought. The test is to read it aloud. If it has energy and still sounds like a person talking, it passed.

`SKILL.md` ends with a quality checklist that covers all of this. The assistant runs through it after every draft.

---

## Repository layout

```
SKILL.md                          # The framework: selection, routing, editorial craft, checklist
references/
  archetypes/                     # One voice definition per archetype
    sage.md  explorer.md  creator.md  caregiver.md  hero.md  rebel.md
    magician.md  innocent.md  everyman.md  jester.md  lover.md  ruler.md
  website-channel.md              # Long-form marketing and landing pages
  linkedin-channel.md             # LinkedIn posts and extraction from source material
  ui-channel.md                   # Tooltips, empty states, errors, buttons, onboarding
  micro-channel.md                # Ambient, per-moment one and two line copy
  language-level.md               # Reader reading-level control (CEFR A2 to C2)
```

Start with `SKILL.md`. Everything else is loaded on demand from there.
