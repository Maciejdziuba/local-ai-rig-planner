# Local AI Rig Planner (skill)

A portable agent **skill** that turns a hardware budget into a concrete local-AI rig
plan: exact GPUs, total VRAM, the open models you can run, realistic tokens/sec, and
an upgrade path.

Built from David Ondrej's interview with **0xSero** on running frontier open models
at home.

## What it does

You say: *"Plan me a $20k local AI rig, I care about speed."*
It returns the GPUs to buy, total VRAM, the models that fit (Qwen, Step, DeepSeek,
GLM 5.2, Kimi…), expected tok/s, and what to upgrade next.

## Use it

**In Claude Code / any agent that supports skills**

```bash
# clone into your skills directory
git clone https://github.com/Maciejdziuba/local-ai-rig-planner
```

Then drop `SKILL.md` where your agent loads skills (e.g. `~/.claude/skills/`), and ask:

> Plan me a local AI rig for $50k, frontier speed.

**In any chat (Claude, ChatGPT, or your own local model)**

Paste the contents of `SKILL.md` into the conversation, then give your budget.

## Companion skill

Already own hardware? Use **[local-ai-model-matcher](https://github.com/Maciejdziuba/local-ai-model-matcher)** —
it reads your actual machine's specs and tells you the best 3 models to run right now.

## Disclaimer

Prices and model specs are planning anchors from the 0xSero podcast (late
2025/2026). Hardware moves fast — verify current prices. Not financial advice.

## License

MIT
