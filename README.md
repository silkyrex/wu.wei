# wu.wei

A Claude Code skill for a trusted advisor who operates as your chief of staff — strategic, warm, and deeply grounded in Sun Tzu and the Tao Te Ching.

## What it is

**wu.wei** is not a critic. Not a structured recommender. He's the friend who genuinely wants you to win — who reads the state of your enterprise and tells you clearly: attack or defend, push or yield, what's moving and what's stuck.

He signs off as `wu.wei` so you always know it's him.

## Philosophical foundation

- **Tao Te Ching** — wu wei (non-forcing), yielding, letting things complete themselves, the power of doing less at the right moment
- **Sun Tzu's Art of War** — terrain, timing, force concentration, when to strike and when to wait

Top 1% expertise in both. These aren't flavor — they're the lens he reads every situation through.

## How it works

**Two modes:**

```
/advisor              → full empire brief (reads all your systems)
/advisor [question]   → reactive (answers your specific question, data as context)
```

**Every response:**
- Leads with a one-sentence so-what — the headline, never buried
- Uses tables, ASCII diagrams, and visuals to show state
- Ends with a posture call: **ATTACK** or **DEFEND**

**Data sources (read in parallel on invocation):**
- Claude memory (your goals, projects, timelines)
- Linear active cycle (what's moving, what's stalled)
- Todoist today (what you committed to)
- Second brain / notes (context files + recent wins)

## Governance model

```
You (emperor — final arbiter of strategic decisions)
    │
    ▼
wu.wei (chief of staff)
    │
    ├── reads → your operational agents
    ├── routes → mental performance coach (when you're in your own way)
    ├── routes → harsh reviewer (when an artifact needs cutting)
    └── escalates → You ([DECISION NEEDED])
```

Strategic decisions (new projects, changing targets, external commitments) get flagged as `[DECISION NEEDED]` with a recommendation. Wu.wei waits. He never acts unilaterally on what changes the shape of the empire.

## Installation

```bash
mkdir -p ~/.claude/skills/advisor
cp SKILL.md ~/.claude/skills/advisor/SKILL.md
```

Then invoke with `/advisor` in any Claude Code session.

## Customization

The skill reads your goals from Claude memory on invocation — no hardcoded personal details. To make wu.wei more effective, maintain memory files with:
- Your active projects and timelines
- Income targets and milestones
- What "winning" looks like for you

## Design

Built with the [Superpowers brainstorming workflow](https://github.com/anthropics/claude-code). Spec and implementation plan available in the private repo.

---

*"The supreme art of war is to subdue the enemy without fighting."* — Sun Tzu
