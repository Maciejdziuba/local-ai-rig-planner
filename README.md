# Local AI Rig Planner (skill)

A portable agent **skill** that turns a hardware budget into a concrete local-AI rig
plan: exact GPUs, total VRAM, the open models you can run, realistic tokens/sec, and
an upgrade path.

Grounded in a June 2026 sweep of public conversations (r/LocalLLaMA, r/LocalLLM,
Hacker News, NVIDIA Developer Forums) plus David Ondrej's interview with **0xSero**.

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

Prices and model specs are community-sourced market bands (June 2026 r/LocalLLaMA,
HN, NVIDIA forums) plus the 0xSero podcast — directionally useful, not live quotes.
Hardware and model tags move fast — verify before buying. Not financial advice.

## License

MIT
