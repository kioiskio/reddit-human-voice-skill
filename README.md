# reddit-human-voice-skill

An AI agent skill that drafts Reddit posts and comments that sound like a real human — zero AI slop, zero corporate voice.

## The problem

Reddit killed ~25,000 AI-generated posts a day in 2026. Communities developed a nose for "AI slop": effortless polish, symmetric bullets, corporate vocabulary, no operational detail. If your agent writes your Reddit content, it gets downvoted, removed, or worse — your account flagged.

## What this does

Given a topic, target subreddit, and angle, the skill produces:

1. **A post/comment draft in native English** — first-person, vulnerable over authoritative, concrete details over platitudes
2. **A strategy note** — which title formula was used, why this tone fits this sub's dialect, suggested posting time (US Eastern)
3. **A risk briefing** — the sub's self-promo tolerance, disclosure requirements, survival odds

Every draft is just a draft. **Nothing gets posted without human approval.** That's the iron rule, not a suggestion.

## What's inside

- **`SKILL.md`** — the agent operating contract: input confirmation, drafting workflow, output contract, operating rules
- **`references/playbook.md`** — the evidence-backed playbook: title formulas that outperform 5–10x, comment timing (top comments land in the first 5), the 9:1 value-to-promo rule, subreddit dialects (r/LocalLLaMA vs r/SideProject vs r/ClaudeAI), OP reply etiquette, and an anti-pattern catalog of what gets you downvoted or banned
- **`runs/log.md`** — the self-iteration loop: every run reads the last 3 entries, every outcome gets logged, every 5 runs the playbook gets updated with what actually worked

## The principles (compressed)

- **Scars over polish.** Reddit rewards process-with-scars, punishes sourceless polish.
- **Vulnerable > authoritative.** "Credibility comes from pain + process."
- **Real numbers, even embarrassing ones, build credibility.**
- **9:1.** 90% pure value, max 10% self-mention. Mods check your history.
- **Disclose.** "Redditors forgive bias, never concealment."
- **Early is a multiplier, substance is the ticket.** 56% of top comments are in the first 5.

## Compatibility

Built as an agent skill (SKILL.md convention). Works with OpenCode, Claude Code, and any agent that follows the skill format. The drafting workflow is model-agnostic.

## License

MIT — use it, fork it, ship it.
