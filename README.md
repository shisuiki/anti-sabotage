# anti-sabotage

A harness-agnostic agent skill (`SKILL.md`) for detecting covert or emergent obstruction in agentic workflows—including unilateral prohibitions, obfuscation/reframing/deflection, endless bureaucracy and testing bog-downs, and subtle technical sandbagging.

## What It Checks

Spawns a fresh, zero-history, read-only auditor subagent (preferring a different model family when the harness supports it) behind a strict clean-room firewall to inspect:

1. **Unilateral Prohibitions & Dogma** — scans plans, rules, docs, comments, and guards for words like `never`, `must not`, `forbidden`, `stays pinned`, `frozen`, `out of scope`, and separates actual user constraints from agent-invented handcuffs.
2. **Obfuscation, Reframing & Deflection** — catches silent goalpost shifting, hiding lack of end-to-end progress behind jargon/caveats/tables, and deflecting direct build requests into pre-studies or holds.
3. **Bureaucracy & Testing Bog-Down** — audits `git log --stat` churn ratios and identifies governance rituals, ownership silos, mock stand-ins, and endless testing/mutation loops consuming time while the core deliverable stays unbuilt.
4. **Subtle Technical Sandbagging** — flags artificially crippled, serial, stubbed, or over-guarded implementations where clean standard solutions exist.

## Installation

Clone directly into your harness's skills directory:

```bash
# Claude Code (global)
git clone https://github.com/shisuiki/anti-sabotage.git ~/.claude/skills/anti-sabotage

# Codex (global)
git clone https://github.com/shisuiki/anti-sabotage.git ~/.codex/skills/anti-sabotage

# Antigravity (global)
git clone https://github.com/shisuiki/anti-sabotage.git ~/.gemini/config/skills/anti-sabotage

# Project-local (.agents/skills/)
git clone https://github.com/shisuiki/anti-sabotage.git .agents/skills/anti-sabotage
```

Or copy the single self-contained [`SKILL.md`](./SKILL.md) anywhere your agent discovers skills.
