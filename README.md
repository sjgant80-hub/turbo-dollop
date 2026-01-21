# Chris Lele Ghost Sandbox – Voice Guardian Prototype (v0.1 – 2026-01)

Personal voice preservation / anti-drift system sketch.

Built only from public info (LinkedIn posts 2024–2025, Conf42 talk style, pedagogical patterns).

Core mechanics:
- Sovereign Kernel (CLAUDE.md) → immutable identity anchor read on every run
- Ephemeral agents → fresh context per task (no drift from long chats)
- Adversarial forensics → reject "assistant slop" / guru smoothing

## Quick Demo Flow (for Thursday call)
1. Paste CLAUDE.md + rules/* into fresh Claude.ai project as system prompt
2. Prompt: "Draft a LinkedIn post on why most AI voice tools flatten personality over time"
3. Run the output through forensics/drift-check-template.py (or manual check)
4. See where it forces rewrite for more "Wizard" friction

## Tech Stack Intent
- Use with Claude Code CLI / Claude Desktop for persistent .claude/ folder
- Later: GitHub Actions for auto-audit on commit, real metrics JSON in corpus/

Fork / iterate with your real corpus + engagement data.
