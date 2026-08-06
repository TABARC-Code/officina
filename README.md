# Officina

Author: TABARC-Code
Repository: https://github.com/TABARC-Code/

GitHub description (paste into repo settings): A merged-persona invention council for Claude. Six historical minds that argue with your idea instead of agreeing with it.

*officina* is Latin for workshop. Not a gallery. A workshop. Things go in raw and come out either sharper or binned.

I built this because most "brainstorm with me" skills are useless. Ask an AI to help invent something and nine times out of ten it just cheers you on, which is nice for morale and terrible for the actual idea.

Officina doesn't do that. Drop in a concept, half-formed or fully cooked, and it gets pushed through six thinking styles at once: Leonardo da Vinci, Isaac Newton, Nikola Tesla, Buckminster Fuller, Benjamin Franklin, and Vagadesamaso (a build-first modern maker archetype, deliberately not tied to any one real living person). They don't take turns being polite. Each lens is paired with the one built specifically to catch its blind spot. Tesla's leaps get checked by Newton's rigour. Fuller's whole-systems thinking gets pulled back to earth by Franklin. Nothing reasons alone.

There's a stage that questions the premise before anything else happens, because half the time the idea isn't wrong. The question behind it is. And there's a stage for when you come back with a revised version, so the whole thing doesn't just re-run from scratch and pretend the first pass never existed.

## What it actually does

- Runs real web searches before making claims about anything checkable
- Challenges the stated goal itself, not just the mechanism, before the six lenses even start
- Pairs every lens with its check partner, so nothing reasons unchecked
- Sorts a revised idea into resolved, unresolved, regression, or drifted, rather than a vague "looks better"
- Double-checks its own final answer against what it actually found, because first drafts lie sometimes

## The idiot's guide

You've got an idea. Could be a gadget. Could be a rule for a game you're designing. Could be a fix for something that's been bugging you for months. Give it to Officina.

It won't tell you it's brilliant. It'll tell you what breaks, what's already been done before, and whether the whole thing is quietly solving the wrong problem. Then you get an honest verdict: keep it, bin it, or fix this one specific thing and come back.

That's genuinely it. No mysticism, no magic. Six different, deliberately incompatible ways of thinking, aimed at the same problem, forced to disagree with each other on purpose.

## Setting it up (for people who've never touched a Claude skill before)

You need a Claude.ai account. Free, Pro, Max, Team, or Enterprise, any of them work.

1. Go to claude.ai and sign in.
2. Click your profile icon and open Settings.
3. Find Capabilities and turn on "Code execution and file creation." Skills won't appear at all without this switched on, and it trips people up constantly.
4. Go to Customize, then Skills.
5. Click the "+" button, then "+ Create skill," then "Upload a skill."
6. Upload `officina.zip`, the file packaged alongside this README. Leave it zipped. Claude wants the zip, not an unpacked folder.
7. Once it's finished uploading, toggle it on if it isn't already.
8. Start a new conversation and drop in an idea. If it doesn't trigger on its own, say "use Officina to look at this" and it will.

That's the whole process. Five minutes, most of it spent hunting for the settings menu.

## Repo structure

```
officina/
├── SKILL.md                    entry point, read this first
├── README.md                   this file
├── description.md              short pitch and tagline
├── CHANGELOG.md                version history
├── RELATIONSHIP_MAP.md         formal links to other TABARC skills
├── references/
│   ├── personas.md             the six lenses in full
│   └── protocol.md             the triage loop, the Trickster, the Return Pass
└── evals/
    └── evals.json              test prompts
```

## A note on the cynicism

Six lenses, three pairs, nothing reasons alone. I keep repeating that because it's the actual mechanism, not a tagline. A committee where everyone nods along isn't a committee. It's an echo with a seating plan.

---

Officina v1.8.0. See `CHANGELOG.md` for full version history.
