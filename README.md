# Free n8n AI Workflows (local LLM, $0 to run)

Ready-to-import [n8n](https://n8n.io) workflows that use a **local LLM via [Ollama](https://ollama.com)**, so there are no OpenAI bills and your data never leaves your machine.

| Workflow | What it does |
|---|---|
| [AI Morning Brief](workflows/ai-morning-brief.json) | Reads your RSS feeds at 7am and posts a 5-bullet "what matters today" brief to Discord |
| [AI Lead Qualifier](workflows/ai-lead-qualifier.json) | Scores contact-form leads 1–10, summarizes them, drafts a first reply, and pings you on hot ones |
| [Website Change Watcher](workflows/website-change-watcher.json) | Watches any page hourly and explains *what* changed (pricing, wording, listings) in plain English |

## Quick start

1. Install Ollama, then run `ollama pull llama3.2`
2. Run n8n (`npx n8n` or Docker)
3. In n8n, go to **Workflows → Import from file** and pick a `.json` from `workflows/`
4. Replace `REPLACE_ME` in the Discord node with your [Discord webhook URL](https://support.discord.com/hc/en-us/articles/228383668), or swap that node for Slack, email or Telegram
5. Click **Test workflow**, then **Activate**

> If n8n runs in Docker and Ollama runs on the host, change `http://localhost:11434` to `http://host.docker.internal:11434`.

## Want one built for you?

**Siren Labs** builds custom AI automations: inbox triage, lead routing, research bots, content pipelines, and chat-on-your-docs. They're self-hosted, private, and fixed-price.

👉 **[Order a custom automation, from $75](https://ko-fi.com/4siren123/commissions)**

Made by the team behind [SIREN](https://messagegabrielhere-lgtm.github.io/doomcon/), a live AI-risk dashboard · [@SIRENutf6](https://x.com/SIRENutf6)

MIT licensed. Use, fork, and sell builds on top of these freely.
