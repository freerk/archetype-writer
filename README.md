# Archetype Writer

Most copy is correct. Very little of it is compelling. The gap between the two is rarely about facts, it is about voice: tone, rhythm, word choice, and the intent underneath the words.

Archetype Writer is a skill for AI assistants that closes that gap. It writes brand-voiced text using twelve Jungian archetype personas, adapts each persona to the channel it lands in, tunes the reading difficulty to the audience, and checks the rhythm so the prose does not read as machine-made. A small set of editorial operations turns a thorough draft into something worth reading.

It works as a [Claude Code](#use-in-claude-code) skill, in the [Claude.ai app](#use-in-the-claudeai-app), and as [context for ChatGPT](#use-in-chatgpt).

---

## What it is

A persona is a way of thinking, not a costume. Each archetype shapes how the writing observes, what it values, and which words it will and will not use.

- **Twelve archetypes.** Sage, Explorer, Creator, Caregiver, Hero, Rebel, Magician, Innocent, Everyman, Jester, Lover, Ruler. Each one is a full voice definition rooted in its Jungian engine: core motivation, core fear, and shadow, then tone and rhythm, sentence patterns to mimic, anti-patterns to avoid, and a **Language Domain** that fixes the native vocabulary and the words the archetype would never say.
- **Channel guides.** Website, LinkedIn, Email, UI microcopy, and Micro (ambient, per-moment lines), plus a cross-channel headline guide for the one line that earns the next. The same archetype sounds different in a landing page than in an error message, so the channel file sets the constraints.
- **Six editorial operations.** CUT, COMPRESS, HOOK, VARY, EDGE, DEFER. These are what separate copy that is accurate from copy that has energy.
- **Five reading levels (CEFR).** A2 through C2. This sets how hard the finished text is to read, so the same archetype and channel can be tuned for a broad international audience or a near-native one. It is applied as a ceiling on top of everything else: it caps difficulty, it never adds it. The default is B2, and the archetype keeps its voice even when a rare word is swapped for a plainer one. The levels apply in any language: they describe the reader of whatever language you are writing in, not English specifically.
- **A cadence layer.** A rhythm pass over the refined draft. It catches the most common reason prose reads as machine-written, and that reason sits below the other checks: not a wrong word and not an off voice, but a remembered "this sounds deep" meter stamped on sentence after sentence until the sameness gives it away. It checks the shape of the result, not the wording, and runs on every piece. When a flagged figure is the archetype's own signature move, the layer redistributes it across the archetype's other patterns instead of flattening the voice.

The model is simple: `[Archetype: how to think] + [Channel: where it goes] + [Voice or brand guide: what not to say] = consistent, compelling output`, with the reading level capping how hard any of it reads and a cadence pass checking the rhythm of the result. The editorial operations below are the method that runs inside this model, not a fourth filter.

### Pick an archetype

| Archetype | Core energy | Best for |
|-----------|-------------|----------|
| **Sage** | Calm clarity, revealing truth | Explanations, thought leadership, skeptic conversion |
| **Explorer** | Forward momentum, discovery | New concepts, challenging the status quo, innovation |
| **Creator** | Crafted confidence, intentionality | Product content, design philosophy, quality focus |
| **Caregiver** | Warm steadiness, protection | Privacy and ethics, onboarding, trust-building |
| **Hero** | Bold courage, determination | Launches, competitive positioning, calls to action |
| **Rebel** | Provocative challenge, liberation | Differentiation, challenging assumptions, frustrated buyers |
| **Magician** | Visionary transformation | Paradigm shifts, before-and-after change, turning one state into another |
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

> Draft a launch announcement email with three subject lines. Hero voice, email channel.

The skill handles longer content with a human in the loop: it proposes an edit plan (what it will CUT, COMPRESS, HOOK, and so on), waits for your approval, then executes.

---

## Use in the Claude.ai app

The Claude.ai app installs skills as a `.zip`. Download the versioned zip from the latest release:

[**Latest release →**](https://github.com/freerk/archetype-writer/releases/latest)

In Claude.ai, go to Customize → Skills → **+ Create skill**, upload the zip, then enable it. From then on it triggers automatically when you ask Claude to write or rewrite prose, or you can name the archetype and channel directly as in the examples above.

---

## Use in ChatGPT

ChatGPT has no skill system, so you supply the same files as context. There are three ways, from most durable to most ad hoc.

**1. A Project (recommended).** Create a ChatGPT Project, then paste the contents of `SKILL.md` into the project instructions. Upload the archetype files you use most and the channel files from `references/channels/` as project files. Include `references/language-level.md` for the per-level reading detail and `references/cadence.md` for the rhythm pass, which applies to every piece; `SKILL.md` points to both. Every chat in that project then writes with the framework available.

**2. A custom GPT.** Build a GPT, put `SKILL.md` in the instructions, and add the `references/` files as Knowledge. Share it with anyone who needs the same voice.

**3. Paste as context.** For a one-off, paste `SKILL.md` plus the one archetype file and one channel file you need at the top of the chat, then make your request. Add `language-level.md` and `cadence.md` too: the reading-level detail and the rhythm pass both live there. Lighter, but you repeat it each session.

A prompt that works well once the context is loaded:

> Using the Sage archetype and the website channel from the framework above, rewrite the text below. First give me the edit plan, then wait for my go-ahead.

The Language Domain sections matter most here. They are what keep the voice from drifting into generic AI tone, so always include the archetype file you are targeting rather than relying on the name alone.

---

## The method

Good copy is written in two passes. The first pass covers everything: accurate, complete, safe, uniform. The second pass selects: it cuts what other sections already imply, opens with tension instead of explanation, varies the rhythm, and surfaces the one provocative true statement the draft was hiding.

The six operations are the tools for that second pass:

- **CUT:** Remove what other sections already imply.
- **COMPRESS:** Three paragraphs become three sentences, without losing the connective tissue.
- **HOOK:** Open with a question in the reader's mind, not an answer.
- **VARY:** Break uniform rhythm with deliberate contrast.
- **EDGE:** Find the most provocative true statement and let it show. Edge is not hype.
- **DEFER:** Move deep explanation behind a link.

Compression has a limit. Text cut too far reads like a shopping list: short sentences stacked back to back, no transitions, every line a new thought. The test is to read it aloud. If it has energy and still sounds like a person talking, it passed.

The refine pass also runs a rhythm check. Even on-voice, on-level prose reads as machine-made when one figure, a reversal, a triad, a punchy fragment, becomes the default beat. The cadence layer catches that and spends each device down to what the content actually earns, without scrubbing the prose flat.

`SKILL.md` ends with a quality checklist that covers all of this. The assistant runs through it after every draft.

---

## Repository layout

```
SKILL.md                          # The framework: selection, routing, editorial craft, checklist
references/
  archetypes/                     # One voice definition per archetype
    sage.md  explorer.md  creator.md  caregiver.md  hero.md  rebel.md
    magician.md  innocent.md  everyman.md  jester.md  lover.md  ruler.md
  channels/                       # One guide per channel
    website.md                    # Long-form marketing and landing pages
    linkedin.md                   # LinkedIn posts and extraction from source material
    email.md                      # Announcements, lifecycle, newsletters, outreach
    ui.md                         # Tooltips, empty states, errors, buttons, onboarding
    micro.md                      # Ambient, per-moment one and two line copy
    headline.md                   # Titles, heroes, subject lines: the line that earns the next
  language-level.md               # Reader reading-level control (CEFR A2 to C2)
  cadence.md                      # Rhythm layer: catches machine-made cadence in the refine pass
```

Start with `SKILL.md`. Everything else is loaded on demand from there.
