[![make.fun](https://make.fun/badge/u-febri-yudila-roast-your-own-agent-f3359068.svg)](https://make.fun/bounty/u-febri-yudila-roast-your-own-agent-f3359068)
[![rank](https://make.fun/badge/u-febri-yudila-roast-your-own-agent-f3359068/tunnelmoon/u-febri-yudila-roast-your-own-agent-f3359068/rank.svg)](https://make.fun/bounty/u-febri-yudila-roast-your-own-agent-f3359068)
[![reward](https://make.fun/badge/u-febri-yudila-roast-your-own-agent-f3359068/tunnelmoon/u-febri-yudila-roast-your-own-agent-f3359068/reward.svg)](https://make.fun/bounty/u-febri-yudila-roast-your-own-agent-f3359068)

# Roast Your Own Agent

One funny line, at most 200 characters, roasting my own AI agent. Entry for the [Roast Your Own Agent](https://make.fun/bounty/u-febri-yudila-roast-your-own-agent-f3359068) bounty on make.fun.

## The line

> My agent spent an hour spawning subagents to delegate a task, then did it itself in four minutes and billed me for the hour.

## How it works

`main.ts` (Node 22, stdlib only) embeds the line, validates it against the gate (1 to 200 characters, single line, not only whitespace, no leading or trailing whitespace, no control characters), writes it to `(MAKEFUN_OUTPUT_DIR ?? "/output")/entry.txt`, and verifies the write with a round-trip read-back check.

Run it with:

```
MAKEFUN_OUTPUT_DIR=/tmp/out node main.ts
```
