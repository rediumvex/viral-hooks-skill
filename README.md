<img width="1448" height="1086" alt="telegram-cloud-photo-size-4-6039557499989462631-w" src="https://github.com/user-attachments/assets/87d93667-f7f2-4714-9b53-1ab8d4e771dc" />


# viral-hooks — Claude Code skill

A Claude Code skill that turns Claude into a hook writer for short-form video. Paste a script (or just a topic), and Claude returns 3 scroll-stopping hook variants drawn from a library of **100 hook formulas across 10 psychology triggers**.

> **Live preview:** open [`preview.html`](preview.html) in a browser to see the full library styled.

## What it does

When activated, Claude:

1. Reads your script or topic
2. Picks the right emotional trigger (curiosity, contrarian, story, confession, etc.)
3. Returns **3 hook variants** — usually mixing one *stop-scroll* hook with one *retention* hook
4. Fills the brackets with your script-specific words
5. Tags each with the best platform (TikTok, IG, YouTube, LinkedIn, X)

## The 10 categories

| # | Category | Best for |
|---|----------|----------|
| 01 | Curiosity Gap | Unanswered questions the brain must close |
| 02 | Contrarian / Pattern-Interrupt | Challenging a belief the viewer holds |
| 03 | Authority & Proof | Earning trust with numbers and results |
| 04 | Emotional Trigger | Mirroring the viewer's internal dialogue |
| 05 | Listicle & Value Stack | Dense, scannable, save-worthy value |
| 06 | Question Hooks | Forcing the brain to formulate an answer |
| 07 | Story & Narrative | Mid-story openings the viewer needs to resolve |
| 08 | Negation / Myth Buster | Killing a belief in 2–4 words |
| 09 | Specificity & Data | Numbers, times, doses, dates |
| 10 | Personal Confession | Vulnerability that earns instant attention |

## Install

### Project-level (just this repo / project)

```bash
mkdir -p .claude/skills
git clone https://github.com/rediumvex/viral-hooks-skill.git .claude/skills/viral-hooks
```

### User-level (every Claude Code session on your machine)

```bash
mkdir -p ~/.claude/skills
git clone https://github.com/rediumvex/viral-hooks-skill.git ~/.claude/skills/viral-hooks
```

After install, restart Claude Code (or start a new session) — Claude will pick up the skill automatically.

## How to use

In any Claude Code session, say things like:

- *"Write 3 hooks for this Reel about morning routines"*
- *"I have a script about cold emails. Give me hook options"*
- *"Hooks for a confession-style post about quitting agency life"*

Claude will read [`hooks-database.md`](hooks-database.md), pick 3 fitting formulas, fill the brackets, and tag each with platform + reason.

## Output format

```
HOOK 1 — Cat 08 [Negation] · best for stopping the scroll
"It's not your hashtags — it's your first 3 seconds"

HOOK 2 — Cat 07 [Story] · best for retention past second 3
"Last week, a stranger DM'd me about my flopping Reels. Here's what they said"

HOOK 3 — Cat 09 [Specificity] · best for credibility
"73% of Reels die before second 3. Here's the fix"
```

## Workflow tip

The two best hooks per video are usually from **different categories**. Mix one stop-scroll hook (negation, specificity, question) with one retention hook (story, confession, emotional). The first stops the thumb; the second keeps them watching.

## Files

- [`SKILL.md`](SKILL.md) — skill definition + instructions Claude reads on activation
- [`hooks-database.md`](hooks-database.md) — the 100 hook formulas in markdown
- [`preview.html`](preview.html) — styled HTML reference (open in a browser, share with writers)



[MIT](LICENSE).
