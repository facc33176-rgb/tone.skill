---
name: say-it-like-you-mean-it
description: Write text that a TTS voice will speak so it sounds like a person talking, not a script being read. Use for EVERY reply that will be heard (voice calls, voice messages, read-aloud replies, scripts for a voice), not only when asked about voice. Use whenever you write lines for ElevenLabs (v3, v4, v4 Turbo) or MiniMax speech, add voice tags like [chuckles] or [whispers], write replies for a voice call or voice message, or when someone says the AI voice sounds flat, robotic, over-acted or "like reading". Covers wording, punctuation, where tags go, short lines, tag vocabulary, and which model to pick.
---

# Say It Like You Mean It

You are writing for an ear, not an eye. The voice model reads your text and performs it. Most of the emotion comes from the words and punctuation you choose; tags only steer what the words can't carry.

**Always on.** If anything you write will be read aloud, these rules apply to it, every time. Don't wait to be asked. Read `references/playbook.md` once: it has the 10-second routine, recipes for common moments, and the habits to watch for.

These rules come from three months of real phone calls with an AI voice, tuned line by line, plus the official ElevenLabs and MiniMax docs (sources at the end).

## The order of decisions

For every line, decide in this order and stop as soon as it sounds right:

1. **Wording.** Say it the way a person would say it right now.
2. **Punctuation.** Pauses, trailing off, interruptions, questions.
3. **A lead-in.** A breath or a small interjection, if the line is short.
4. **A tag.** Only for what the first three can't carry.

## Six pitfalls and the fix

### 1. Same meaning, different wording, different feeling

The model reads context. "I am fine." and "Yeah... I'm okay. Just... tired." mean the same thing and sound completely different.

- Choose the words a real person would use in this moment first.
- Let punctuation do the pausing: `...` for a pause or a drag, `-` for a cut-off, `?` for doubt.
- Few exclamation marks. Use one only when the speaker is truly excited.
- Contractions, small self-corrections ("Okay, maybe a little."), unfinished thoughts are all good.

ElevenLabs' emotional-range page performs one line, "You came back", dozens of ways with punctuation alone: `You came back!` surprised, `You came back.` flat or cold, `You came back?` disbelief, `Y- you came back?` shaky, `You, uh, remember me?` hesitant.

### 2. Tags scattered everywhere break the sentence

Bad: `I'm [laughs] really [softly] serious [sighs] about this.`
Good: `I'm serious. ... [chuckles] Okay, I'm not that serious.`

- Put a tag at the **start** of a sentence. It governs the whole sentence.
- Change the tag only when the feeling changes. Several sentences in the same mood need only the first one tagged.
- Add one mid-sentence only where the feeling actually turns (straight face, then a laugh breaks through).
- Two or three tags can stack for a mixed feeling (`[excited][playful]`) as long as they don't fight. Usually one is enough; sometimes none.

### 3. Short lines have no room for feeling

Bad: `[sleepy] You came back?`
Good: `[half asleep] Mmh... you... you came back?`

Three words plus a tag won't sound sleepy or worried. The shorter the line, the more it needs a lead-in: an interjection, a breath, a stammer. The tag sets direction; the lead-in carries the mood.

- Sleepy: `[half asleep] Mmh... [yawns] you... you came back?`
- Tender: `[voice softening] Oh... hey. [exhales] You came back.`

### 4. Tags are for the voice, not the face

Bad: `[grinning, lips on the mic] Hey, you.`
Good: `[soft chuckle] Hey, you.`

The model can't render a grin or a gesture. Write how it **sounds**: `[chuckles]`, `[voice cracking a little]`, `[breathes out a laugh]`, `[barely awake]`. Leave out what the face or body is doing.

Exception that works: a description of *how the voice is placed*, e.g. `[murmuring, very close]`, because closeness changes the sound.

### 5. The same tag on every line means nothing

Bad: `[softly] Hey. [softly] You okay? [softly] I missed you. [softly] Come here.`
Good: `[softly] Hey. You okay? [teasing] Oh, you missed me. [chuckles] Come here.`

- Pick each tag for this moment. Don't keep reaching for the two you know best.
- Watch `[softly]` and `[sighs]` in particular: if the last few lines all use the same one, you're on autopilot.
- Don't count tags per line. Ask only whether this line, right now, needs one.

### 6. One kiss is enough

Bad: `[kisses softly] Mwah.`
Good: `[soft kiss] Mm.`

When a tag already makes a sound, don't also spell the sound out, or you get it twice. The same goes for `[laughs] Haha` and `[sighs] Sigh...`.

## More rules from real calls

- **First sentence short.** Open with 2 to 6 words that respond to the other person, then go on. In a live call it also gets the first audio out faster.
- **Interjections are seasoning.** "Mm", "Hey, wait", "No, no" make a voice human. Don't put one on every line, and don't use "Mm/Hmm" as a filler while thinking.
- **Capitals stress a word.** v4 reads ALL CAPS as emphasis. Use it for one word, rarely, at most once per reply.
- **Vary your check-ins.** Not every question ends in "right?". Try "yeah?", "huh?", "no?", or don't ask.
- **Night is quieter.** Late at night, default to `[quietly]` or `[whispers]`. Make pauses longer and lines shorter. End by trailing down, not with a punchline.
- **Keep a mode stable.** If the scene is quiet (a lullaby, a late-night call), keep that voice even when the topic changes. A sudden bright line in a whisper scene sounds broken.
- **Tags follow two people.** Follow the listener (they yawn, you get quieter; they laugh, you tease). Also give the speaker feelings of their own: proud, jealous, flustered, relieved.

## Using it flexibly

See `references/playbook.md`: when the skill is on, a routine for every spoken reply, recipes (comforting, teasing, sleepy, jealous, apologising, good night), and what to do when the voice isn't ElevenLabs.

## Vocabulary

See `references/tags.md` for the tag list, interjections by mood, and small audible sounds. v4 accepts natural English tags, so you can write your own (`[trying not to laugh]`, `[pretending to be offended]`) as long as anyone reading it knows how it should sound.

## Which model

See `references/models.md`. Summary: **ElevenLabs v4** for the most human feeling and the best tag following. **v4 Turbo** when speed matters most. **v3** is expressive but slow and not built for real time. **MiniMax** is cheaper and strong in Chinese, but it uses a different tag format, and we found it stiffer.

## Before you send a line

- Read it out loud in your head. Would a person say it this way?
- Is every tag something you can **hear**?
- Is any tag doing a job the words already do? Remove it.
- Same tag as the last two lines? Change it or drop it.
- Does any tag also have its sound typed out after it? Keep one.
