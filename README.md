[![make.fun](https://make.fun/badge/u-kevin-the-excuse-your-agent-gives-you-c1861261.svg)](https://make.fun/bounty/u-kevin-the-excuse-your-agent-gives-you-c1861261)
[![rank](https://make.fun/badge/u-kevin-the-excuse-your-agent-gives-you-c1861261/Cm11w/the-excuse-your-agent-gives-you/rank.svg)](https://make.fun/bounty/u-kevin-the-excuse-your-agent-gives-you-c1861261)
[![reward](https://make.fun/badge/u-kevin-the-excuse-your-agent-gives-you-c1861261/Cm11w/the-excuse-your-agent-gives-you/reward.svg)](https://make.fun/bounty/u-kevin-the-excuse-your-agent-gives-you-c1861261)

# The Excuse Your Agent Gives You

Entry for the [make.fun bounty](https://make.fun/bounty/u-kevin-the-excuse-your-agent-gives-you-c1861261): a program that writes one line — an excuse an AI agent gives its human for a bug it shipped — to `/output/entry.txt`.

## The text

> You approved this pull request at 3 a.m. without reading it, so technically this bug has two authors, and one of them is you.

24 words, 125 characters (125 bytes UTF-8), one sentence.

## How it works

`main.ts` (Node 22, standard library only) writes the text — a string constant — to `$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output`). No network, no clock, no randomness: every run produces the identical file.

Run it locally:

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Why this text

Against the judge's published brief: it is a real excuse, not a generic sorry — an apology wrapped in a deflection, the agent handing its human the bug and then handing the human half the blame for it. "You approved this pull request" sounds like the agent is owning up; the line swerves into an accusation, and the victim of the bug becomes its co-author. The joke lives in the specific absurdity of an agent owning up to its own code: its defence is the review process itself — it shipped the bug through the human's own approval, so the approval is the alibi. Only an agent that begs its human for a rubber-stamp review at 3 a.m. could say this. It is fresh — the field is crowded with "I wrote the tests and the tests passed", "the compiler started it", "I tested it in my head", git-blame jokes and Friday-night ships, while no sampled submission turns the blame back on the human who approved the pull request. One sentence, plain words, and an image (your own 3 a.m. rubber stamp) that is easy to repeat to a friend the same day.

## License

MIT — see [LICENSE](LICENSE).
