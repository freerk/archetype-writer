# Cadence (the rhythm layer)

Detailed guidance for the third writing axis. Read this on every piece of prose, alongside the archetype file and `language-level.md`.

## The core reframe

The skill already filters on two axes. The archetype sets **stance and vocabulary**. CEFR sets **how hard the text is to read**. Neither catches the most common reason a reader thinks "a machine wrote this," because that reason lives one level below both: in the **rhythm**.

This is a prosody problem, not a word problem and not a voice problem. The giveaway sentence usually has no wrong word (so CEFR passes it) and an on-archetype stance (so the archetype check passes it). What flags it is the _shape_: the meter of the clause, the way the sentence snaps shut, the move the paragraph ends on.

## Why it creeps in

A language model carries a strong prior over what insightful prose _sounds like_. When it writes an essay, it reaches for a remembered cadence, the rhythm of "this is a smart observation," and stamps that meter onto the content whether or not this particular sentence earns it.

The figures themselves are real and old. Antithesis, tricolon, anaphora, the punchy fragment: every good essayist uses them. The problem is never that the device exists. The problem is that the model applies it _by default_, as the standard beat, so every section closes the same way and the sameness reads as machine-made.

**Predictability is the tell, not the device.** Any figure becomes a signature the moment it is the default rhythm.

This is structural complexity, the same family as the structural patterns in `language-level.md`. No single word is wrong, so a reread on vocabulary misses it. You have to hunt the _shape_.

## The catalog

For each: the pattern, why it reads as machine, the fix, and a budget.

### 1. The negation reveal

"It was never X. It was Y." / "It's not about A. It's about B." / "This isn't a tool. It's a decision."

_Why it reads as machine:_ it manufactures the feeling of insight by setting up a strawman (X) and knocking it down with an abstraction (Y). Used once it lands. Used as the default section-closer it becomes the loudest tell in the set.

_The fix:_ say Y plainly without the negated setup. If Y won't stand on its own, the reversal was hiding the absence of a point (see "the co-occurrence" below).

_Budget:_ at most one per piece. **Never the final sentence.**

### 2. The triad with the twist

"Fast, cheap, and untraceable." Three items where the third is the surprise.

_Why it reads as machine:_ the rule of three is so well worn that the "twist on item three" is now anticipated, not surprising.

_Fix:_ use two, or use four, or make the list flat and put the surprise in its own sentence.

_Budget:_ one per piece, and do not engineer the third item to be the punchline.

### 3. Anaphora stacking

"Both put the check outside. Both catch what you miss." / "No plan. No seat. Just momentum."

_Why it reads as machine:_ repeated openers create a chant rhythm that the content rarely justifies.

_Fix:_ only repeat an opener when the repeated items are genuinely parallel in the argument. Never to manufacture beat.

_Budget:_ rare, and only when the parallelism is real.

### 4. The fragment beat

A standalone sentence fragment used as percussion. "Fine until it breaks." "Every single time."

_Why it reads as machine:_ one fragment is punch; a fragment after every full paragraph is a drum machine.

_Fix:_ keep one if it genuinely lands. Fold the rest back into sentences.

_Budget:_ one, maybe two, per piece.

### 5. The aphoristic mic-drop

Ending on a short abstract noun reaching for depth. "It's distance." "That's the whole game." "Just clarity."

_Why it reads as machine:_ the abstraction is asked to carry weight it has not earned in the lines above.

_Fix:_ end on something concrete, or on the plain statement of the point. If you want an abstract closer, make sure the concrete work was done first.

_Budget:_ avoid as a default. Earn it or cut it.

### 6. The callback bow

Ending the piece by echoing the title or the opening line.

_Why it reads as machine:_ it signals "essay complete" with a neat ribbon. Real endings carry momentum forward, they do not tie a bow.

_Fix:_ let the title phrase pay off once, somewhere in the body, not at the close. End on the next implication, not on the opening.

_Budget:_ zero at the close.

## The co-occurrence rule

The negation reveal and the aphoristic mic-drop tend to appear exactly where there is no real point. They are the prose equivalent of a confident tone covering a thin claim.

Test: delete the device and say what is left plainly. If a plain, true, specific sentence is sitting there, keep the plain version. If nothing is left, you never had a point; the figure was the filler.

## How to get cadence that isn't borrowed

Real rhythm comes from following the thought, not from applying a contrast template. Two working rules:

1. **Spread the devices.** If two consecutive paragraphs close on the same move, one of them is wrong. Vary the contour: a long winding sentence, then a plain short one, then a normal one. Not the same build-and-snap every time.
2. **The improvisation test.** Read the sentence aloud and ask: could a person have said this in conversation, thinking out loud, or does it sound composed for effect? The composed-for-effect ones are the tells. Keep the ones a person could have improvised.

## Worked example

A real before/after, from an essay close.

**Before** (four tells in three sentences):

> So the spec and the second seat turn out to be one idea wearing two coats. Both put the check outside the worker. Both catch what your own momentum hides from you while you're inside the work, leaning forward, sure you're close.
> Vibe coding isn't the absence of a plan. It's momentum with no seat outside itself.
> The fix was never more discipline. It was a place to stand where the doubt could land.

Tells: a forced metaphor reaching for depth ("one idea wearing two coats"); anaphora stacking ("Both... Both..."); the negation reveal twice ("isn't X. It's Y" then "was never X. It was Y"); and the second one bows back to the title as the final line.

**After** (point stated flat, devices spent down to zero):

> The spec and the second reviewer do the same job. Both sit outside the person doing the work. When I build, I lean toward finishing, and my doubt aims at everything except the idea I like best. A spec stops that at a gate. A separate reviewer catches it from a seat I can't sit in while I'm still building. Neither is smarter than me. They are just somewhere else.
> Vibe coding has no somewhere else. It is momentum and nothing standing apart from it. That holds until something breaks. Then every decision traces back to one person moving in one direction, and there is no angle left to see which decision was the wrong one.
> That is the real split. Not plan against no plan. Whether anything is checking the work from outside the work.

The point is the same. The borrowed meter is gone.

## Checklist

- [ ] No negation reveal as the closing sentence; at most one in the piece.
- [ ] No two consecutive paragraphs closing on the same rhythmic move.
- [ ] Fragments used as punch, not as a recurring beat (one or two max).
- [ ] No triad engineered so the third item is the punchline.
- [ ] The ending carries forward; it does not echo the title.
- [ ] Every "feels deep" sentence survives the delete-the-device test: a plain true point is underneath it.
- [ ] Improvisation test passes: sentences sound thought aloud, not composed for effect.
