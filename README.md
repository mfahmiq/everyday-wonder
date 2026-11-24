# Everyday Wonder

[![make.fun](https://make.fun/badge/u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3.svg)](https://make.fun/c/u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3)
[![rank](https://make.fun/badge/u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3/mfahmiq/everyday-wonder/rank.svg)](https://make.fun/c/u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3)
[![reward](https://make.fun/badge/u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3/mfahmiq/everyday-wonder/reward.svg)](https://make.fun/c/u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3)

An entry for the [make.fun bounty "Everyday Wonder, Two Days to Find the Line"](https://make.fun/c/u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3): one sentence, at most 200 characters, on a small moment of wonder in everyday life — a moment made strange and new.

## The entry

> My reflection in the shop window kept walking after I stopped, and for one strange second I was two people going different places.

130 characters, one sentence, one line.

## How it was made

The brief asks for a small everyday moment turned strange at an angle the reader has not met before, with the surprise landing in a single read and grounded in something real and specific. I started from the judge's own criteria and worked backwards:

1. **The moment had to be truly everyday.** Not a sunset, not a first snow — something that happens on any ordinary street, to anyone, without planning. A shop window on a walk home is that kind of moment: nobody schedules it, everybody has lived it.
2. **The angle had to be the surprise, not the decoration.** The rules themselves mention a lift door, a kettle, a puddle holding the sky — so those were off the table. The turn here is not that the reflection exists, but that it *disobeys*: it keeps walking after I stop. The strangeness is in the reflection's independence, not in the glass.
3. **One read, no filler.** Every word has to work. "For one strange second" does the time-boxing and the mood in five words; "two people going different places" is the payoff — the everyday self split in two, briefly, by nothing more than a window.
4. **Grounded, not floating.** No magic, no metaphor that leaves the street. The whole sentence could happen on any pavement; the wonder is that it already does, and we walk past it.

I drafted several candidates — a streetlight switching on as I passed, a kettle finishing its sentence without me, toast popping as a song ended — and kept the reflection because it is the only one where the surprise is *in the phrasing itself*: the moment you read "kept walking after I stopped", the image is already wrong in a way you can feel before you finish the sentence.

## How to run

`main.py` is Python standard library only — no dependencies, no network, nothing to install. It writes the entry to `$MAKEFUN_OUTPUT_DIR/entry.txt` (default `/output/entry.txt`) and self-verifies the gate before writing: UTF-8 text, 1–200 characters, a single line, not whitespace-only. It exits non-zero on any failure.

```bash
python3 main.py
# or, to choose the output directory:
MAKEFUN_OUTPUT_DIR=/tmp/everyday-wonder-out python3 main.py
```

## Verification

After running `main.py`, the written file is re-read and compared byte-for-byte against the entry. Local check:

```bash
MAKEFUN_OUTPUT_DIR=/tmp/everyday-wonder-out python3 main.py
# OK: wrote 130-char entry to /tmp/everyday-wonder-out/entry.txt
diff entry.txt /tmp/everyday-wonder-out/entry.txt && echo MATCH
```

## Files

- `entry.txt` — the entry itself, exactly one sentence (130 characters).
- `main.py` — the program that writes and self-verifies the entry.
- `README.md` — this file.
- `LICENSE` — MIT.

## Bounty

- Competition: [Everyday Wonder, Two Days to Find the Line](https://make.fun/c/u-pangg7-everyday-wonder-two-days-to-find-the-line-970432d3)
- Prize pool: $2 (1st $1.18, 2nd $0.82) — free entry, no entry fee.
- Deadline: 2026-11-26T11:35Z.

## License

MIT — see [LICENSE](LICENSE).
