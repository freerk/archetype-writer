# Email Channel Guide

Use this reference when writing email a person will actually read in an inbox: announcements, lifecycle and onboarding messages, newsletters, and outreach. Not for raw transactional receipts that carry no voice.

An email is read in a hostile place. It arrives next to dozens of others, most of them ignored. The subject decides whether it opens, the first line decides whether it survives, and the body has one job or it has none.

## Where the voice lives

This file describes the shape of an email, not how each archetype sounds in one. For archetype voice (tone, rhythm, sentence patterns, vocabulary, anti-patterns), read the archetype file at `references/archetypes/<name>.md`. The Sentence Patterns and Language Domain sections there are the canonical voice references; apply them within the rules below.

## The anatomy

An email is a stack, and each layer has one job.

1. **Subject line.** Earns the open. Write it last, open a gap, keep it roughly under 50 characters. A subject line is a headline; read `references/channels/headline.md` for how to write it.
2. **Preview text (preheader).** The first ~90 characters the inbox shows beneath the subject. A *second* hook that extends the subject, never a repeat of it. Leave it blank and the inbox fills it with the first body line, usually badly.
3. **Opening line.** Earns the read. Tension before context, the HOOK operation. Never open with "I hope this email finds you well" or a restatement of the subject.
4. **Body.** One idea. The point first, the support under it, the detail last or deferred to a link (DEFER). Short paragraphs, generous whitespace, scannable on a phone.
5. **One primary call to action.** A single thing you want the reader to do, stated plainly and matched to the consequence ("Start your trial", not "Click here"). A second, lower-commitment action is fine. A third is noise.
6. **Sign-off.** Human, brief, in voice.

## One email, one job

The fastest way to kill an email is to ask it to do three things. Pick the single outcome that matters and cut everything that does not serve it. If two outcomes both matter, that is two emails.

## Length

- Most emails: 50 to 150 words of body. Shorter than the writer wants it to be.
- Newsletters and announcements can run longer, but every section still earns its place and defers depth to links.
- If the reader has to scroll twice to find the point, the point was buried too deep.

## Workflow

- **Short, single-purpose emails** (an announcement, an onboarding step, a piece of outreach): write directly and show 2 to 3 variants, each with 2 to 3 subject-line options. The author picks or mixes.
- **Campaigns and longer sends** (a sequence, or a newsletter built from source material): propose a plan first (purpose, audience, the one action, the structure), wait for approval, then write. Same human-in-the-loop sequence as the website and LinkedIn channels.

## Output format

```
**[Email purpose and audience]**

Subject options:
1. "[subject A]"
2. "[subject B]"
3. "[subject C]"

Preview text: "[the second hook, extends the subject]"

---

[Opening line that creates tension]

[Body: one idea, short paragraphs, the point first]

[Primary CTA]

[Sign-off]
```

## Quality checks

- [ ] One email, one job: a single primary action.
- [ ] Subject earns the open and passes the headline checks (`references/channels/headline.md`).
- [ ] Preview text extends the subject instead of repeating it.
- [ ] Opening creates tension, not "I hope this finds you well".
- [ ] Archetype voice is recognisable (verified against the archetype's Sentence Patterns and Language Domain).
- [ ] CEFR ceiling respected (default B2): no rare words or opaque constructions above the target.
- [ ] Passes `references/cadence.md`: no machine-made rhythm, especially in the subject and the opening.
- [ ] Body is scannable: short paragraphs, depth deferred to links.
- [ ] Read aloud: sounds like a person writing to one reader, not a broadcast.
