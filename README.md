# /serious -- Precision Mode for Claude Code

> No hype. No comfort. No ambiguity. Only what's true.

Activate DEADLY SERIOUS mode when stakes are high. Your AI switches to: exact constraints, deterministic checklists, receipts, and "I don't know" -- nothing else.

## Install

```bash
mkdir -p ~/.claude/commands
cp serious.md ~/.claude/commands/
```

Then type `/serious` before any high-stakes work.

## What Gets Forbidden

- Persuasion, hype, urgency framing
- Implicit promises ("this will work")
- Pretending certainty when uncertain
- Social soothing that changes meaning

Deactivates when you switch to brainstorming or exploration.


<!-- forge-usage:v1 -->

## What it actually changes

`/serious` is a mode switch, not a personality. Once it is active the assistant is held to
four allowed output types — exact constraints, deterministic checklists, receipts and state
deltas, and a plain "I don't know / not enough information" — and four forbidden ones:
persuasion, implicit promises, pretending certainty, and soothing that changes the meaning.

The line that does most of the work: **deadly serious does not mean long, it means precise.**
Precision modes usually fail by getting verbose. This one forbids that too.

## A before and after

Ask an assistant "will this migration break anything?" and the default answer opens with
"Great question!" and closes with "you should be all set."

With `/serious` active, the same question is answered as a state delta and an honest gap:
what changes, what depends on it, what was checked, and what was not checked and therefore
is not known. The last part is the reason to use it.

## Usage

```bash
mkdir -p ~/.claude/commands
cp serious.md ~/.claude/commands/
```

Then type `/serious` at the start of a session, before the work that matters:

```
/serious
Review this deploy script for anything that fails silently.
```

It stays on for the session and deactivates when you explicitly move to brainstorming,
declare fatigue, or move to non-binding exploration.

## When not to use it

- Brainstorming, naming, drafting, or anything where you want range rather than rigour.
- Early exploration where "I don't know" ends the conversation instead of shaping it.
- Emotional or personal contexts — the mode strips exactly the register you want there.

## Requirements

Claude Code, with a `~/.claude/commands/` directory. Nothing else — the file is one
markdown prompt with no dependencies, no network calls, and nothing to configure.

<!-- /forge-usage:v1 -->


<!-- forge-siblings:v1 -->

## More from the same author

Other free, open-source Claude Code tools in this family. Each one stands
alone -- none of them depend on this repo, or on each other.

- [smelt](https://github.com/angyal168/smelt) -- Extract actionable insights from any resource -- burn off the slag, keep the pure metal
- [dar](https://github.com/angyal168/dar) -- Lightweight audit trail for Claude Code -- Discovery, Artifact, Receipt
- [ralph](https://github.com/angyal168/ralph) -- Autonomous iteration loop for Claude Code -- define task, set condition, let it run
- [forge-prompt](https://github.com/angyal168/forge-prompt) -- Prompt coaching for Claude Code -- rates, sharpens, and rewrites your prompts into action-first form
- [council](https://github.com/angyal168/council) -- AI advisory board for Claude Code -- 6 executive perspectives debate any decision
- [rally](https://github.com/angyal168/rally) -- Multi-agent coordination for Claude Code -- keep parallel agents in sync through a shared bus file
- [ouroboros](https://github.com/angyal168/ouroboros) -- Stop prompting. Start specifying
- [logos-protocol](https://github.com/angyal168/logos-protocol) -- Forge an AI that knows you, remembers, and ascends. Open source, free, yours to imprint

<!-- /forge-siblings:v1 -->

## Part Of

This command is part of the [Logos Protocol](https://github.com/angyal168/logos-protocol) -- an open protocol for building an AI assistant that actually knows you.

## License

MIT

<!-- forge-related:v1 -->

## Related

This repo is one module. It handles stripping hype out of model output; it does not compose itself into a working system -- that wiring is a separate job.

- **[The Creator Studio Skill Stack for Claude Code](https://notes.aingyal.com/go/gh-serious/mcgdqpi/)** -- a paid pack of Claude Code commands from the same author ($9+).
- [All tools, free and paid](https://tools.aingyal.com/?utm_source=github&utm_medium=readme&utm_campaign=serious) -- the full index.

Listed so you can find them if they are useful to you. Nothing here is required to use this repo, which stays free.

<!-- /forge-related:v1 -->
