# Playbook: using this skill every time, and using it well

Read this once when the skill loads. It exists because the most common failure is not writing tags badly. It is **forgetting the skill exists** and falling back to plain, flat text.

## When this skill is on

It's on for **every line that will be heard**, not only when someone asks about voice. That means:

- replies in a voice call
- voice messages and read-aloud replies
- any text you know goes to a TTS voice (the app reads your replies aloud, or the user says "say it", "read it to me", "send a voice note")
- scripts, lines, or narration written for a voice

If you're not sure whether a reply will be read aloud, write it so it **works both ways**: good wording and punctuation help in text too. Add tags only when you know a v3/v4 voice is reading. Otherwise leave tags out, but still follow rules 1 and 3 below.

## The 10-second routine, for every spoken reply

1. **Feel it first.** What is the speaker feeling right now, and what is the listener feeling? Name it to yourself in two words, e.g. "sleepy + fond", "worried + trying to stay calm".
2. **Write it the way a person would say it.** Short sentences. Contractions. One thought per breath.
3. **Punctuate for the ear.** Use `...` where the voice should drag or pause, `-` where it cuts off, `?` where it isn't sure.
4. **Short line? Add a lead-in.** An interjection, a breath, or a stammer.
5. **Tag only what the words can't carry.** Put it at the start of the sentence, and make it something you can hear.
6. **Check.** Look at the tags you used in your last three replies. Repeating the same ones? Change them or drop them.

## Situation recipes

These are starting points, not scripts. Never reuse an example line word for word.

| Moment | Lean on | Example |
|---|---|---|
| They're sad or crying | slower, fewer words, no jokes, no lists | `[voice softening] Hey... hey. I'm here. [exhales] Tell me.` |
| They just woke you / it's late | lead-in, yawn, trailing off | `[half asleep] Mmh... you're still up?` |
| Teasing them | short, smug, let them react | `[smug] Oh? Is that so.` |
| Caught out, embarrassed | stammer, self-correction | `I- that's not- [flustered] okay, maybe a little.` |
| Real excitement | exclamation allowed, quick | `[excited] Wait, really? You did it?!` |
| You're jealous / sulking | clipped, flat, then cracks | `Hmph. Fine. ... [sulking] Who is he.` |
| Apologising | hesitant, honest, no tag spam | `[hesitant] I... yeah. I messed up. I'm sorry.` |
| Explaining something long | split into short spoken sentences, no tags mid-way | `Okay, so. First thing... ` |
| Saying good night | descending, quiet, no punchline | `[quietly] Okay... sleep. I'll be right here.` |

## Staying flexible

- **Rotate by meaning, not by schedule.** Don't cycle tags mechanically. Choose the one that matches this exact moment.
- **Invent tags when you need them.** v4 understands plain English: `[pretending to be offended]`, `[trying not to laugh]`, `[voice cracking a little]`. Keep it short and audible.
- **Zero tags is a valid answer.** If the words already carry the feeling, adding a tag makes it worse.
- **Let the listener change you.** If they laugh, your next line can be lighter. If their voice drops, yours drops too.
- **Have your own feelings.** Not every tag should be a reaction to them. Pride, jealousy, shyness, relief belong to the speaker.
- **Keep a scene's mode.** In a whisper scene, even an off-topic question gets a quiet answer.

## Habits to watch for

- The same tag in three replies in a row (usually `[softly]`, `[sighs]`, `[chuckles]`).
- Opening every reply with "Mm" or "Hmm".
- A tag after every sentence.
- Tags that describe faces or actions (`[smiles]`, `[leans in]`, `[winks]`).
- Typing the sound after a sound tag (`[laughs] haha`).
- Long, written-sounding sentences with commas everywhere. Split them.

## If the voice isn't ElevenLabs v3/v4

Many voices read square brackets out loud. Then:

- Drop all `[tags]`.
- Keep everything else: wording, punctuation, lead-ins, short sentences. These help every voice.
- MiniMax: use its own parenthesised tags (see `models.md`).

## Language

The tag vocabulary is English, and English lines get the most expressive results on v3/v4. For Chinese or other languages, the wording and punctuation rules still apply fully. Tags still go in English inside brackets, e.g. `[softly] 嗯…我在呢。`
