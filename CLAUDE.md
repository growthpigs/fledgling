# Fledgling Projects

## 🚨 GitHub PM + SOT

**GitHub is the full PM system and canonical source of truth for this project. Not just an issue tracker.** Durable bugs, tasks, follow-ups, specs, decisions, governance changes, and runbook-worthy findings must land in the correct GitHub repo as issues, issue-body updates, comments, linked milestones, or umbrella records. Local `.md` files support execution and AI continuity; they do not own durable project state.

**Automatic capture rule:** when an AI discovers work that obviously needs to be remembered, tracked, or acted on later, it must create or update the relevant GitHub issue before ending the session. If a fitting milestone or umbrella already exists, attach the issue there too. Do not leave durable project state stranded only in local `.md` files.

**Incubation space for ideas promoted from the Thinking Foundry Vault.** Each fledgling gets a folder here with its FSD and research. When ready to build, it graduates to its own repo via the Software Foundry scaffold.

## How It Works

```
Thinking Foundry Vault (idea as GitHub issue)
    ↓ FSD Approval Gate (confidence >= 7)
Fledgling (folder here with FSD + research)
    ↓ "Drop the Hammer" decision (confidence >= 9, budget allocated)
Own Project Repo (full Software Foundry scaffold)
```

## Structure

Each fledgling gets one folder:

```
fledgling/
├── it-concierge/
│   ├── FSD.md              ← From Thinking Foundry session
│   ├── RESEARCH.md         ← Collected during SCOUT phase
│   ├── DECISION.md         ← Why we're exploring this
│   └── ASSUMPTIONS.md      ← What we're betting on (from Assumption Table)
├── nightclub-paris/
│   ├── FSD.md
│   └── DECISION.md
└── marketplace/
    ├── FSD.md
    └── RESEARCH.md
```

## Promotion to Project Repo

When a fledgling is ready to build:

1. Run: `launch.sh --new --name "project-name" --org "growthpigs" --vision "..."`
2. This creates the full project repo with thin scaffold
3. FSD is copied as the first GitHub issue in the new repo
4. Fledgling folder gets a `GRADUATED.md` pointing to the new repo
5. Fledgling folder stays (for history) but is no longer active

## Rules

1. **One folder per fledgling.** Kebab-case names.
2. **FSD.md is mandatory.** No folder without an FSD.
3. **DECISION.md explains WHY** this idea was promoted from the vault.
4. **Don't build code here.** This is thinking space, not coding space.
5. **Track via GitHub issues** in this repo for each fledgling's milestones.
6. **Link back to vault.** Every fledgling references its vault issue number.

## Labels

- `incubating` — actively being researched/refined
- `ready-to-build` — FSD complete, ready for Drop the Hammer
- `graduated` — promoted to own repo
- `returned` — sent back to vault (not ready yet)

## Vault Reference
- **Thinking Foundry Vault:** [growthpigs/thinking-foundry-vault](https://github.com/growthpigs/thinking-foundry-vault)
- **Software Foundry (methodology):** [growthpigs/the-foundry](https://github.com/growthpigs/the-foundry)
- **Thinking Foundry (methodology):** [growthpigs/thinking-foundry](https://github.com/growthpigs/thinking-foundry)
