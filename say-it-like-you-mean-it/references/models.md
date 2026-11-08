# Which voice model

Numbers are from our own tests in real use (2026-10 to 2026-11), not official benchmarks. Your network and text length will differ.

## Same line, three ElevenLabs models (tested 2026-10-30)

| Model | First audio, short line | Whole long line generated | Feeling |
|---|---|---|---|
| Eleven v3 | 0.94 s | 4.43 s | Very expressive |
| **Eleven v4** | 1.06 s | 2.93 s | Most emotional; the one we chose by ear |
| v4 Turbo | 0.13 s | 1.41 s | Fastest; flatter |

## What each is good at

- **ElevenLabs v4.** ElevenLabs calls it their most emotive model and says it follows tags more accurately. It reads mood from the text itself, so wording and punctuation matter even more. Our pick for calls and voice messages: most human, and even long lines finish in under 3 s.
- **ElevenLabs v4 Turbo.** Built for speed (ElevenLabs gives a median time-to-first-audio around 150 ms). Choose it when latency matters more than nuance.
- **ElevenLabs v3.** Expressive and understands tags, but slow. ElevenLabs' help center says it is not built for real-time use. Good for pre-recorded clips.
- **MiniMax Speech 2.8.** Cheaper, good Chinese, and it has built-in laughs and sighs. It uses **parenthesised** interjection tags from a fixed list of 19, such as `(laughs)` `(sighs)` `(chuckle)` `(emm)`, and pauses written as `<#0.5#>` (seconds). Square-bracket v3/v4 tags don't apply. To our ears it was stiffer (2026-10-25).

## Practical notes from real calls

- Concurrency: our ElevenLabs plan allowed only 2 generations at once. A third returned 429. Queue requests, don't fire them all at once.
- Split long replies at sentence ends and voice the first sentence alone, so the listener hears something sooner.
- v3/v4 don't support `<break>` tags. Use punctuation (`...`, `-`) for pauses.
- The text model matters as much as the voice. In our calls, the time until the language model's first sentence (3 to 6 s) was usually bigger than the voice's.

## Sources

- ElevenLabs, Best practices / prompting for v3 and v4: ellipses add pauses and weight, capitals add emphasis, tags should clearly describe the voice; no `<break>` on v3/v4.
- ElevenLabs, Eleven v4 launch post and the emotional-range page (one line performed many ways).
- ElevenLabs help center: v3 is not designed for real-time.
- MiniMax Speech 2.8 docs: 19 interjection tags in parentheses, `<#x#>` pauses.
