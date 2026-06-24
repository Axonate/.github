<div align="center">

# Axonate

### One key, every model — AI that fits a small team's budget.

Axonate is a self-hosted, OpenAI-compatible gateway in front of **every model** — real provider
APIs (Anthropic, OpenAI, AWS Bedrock, Azure…) **and free local models** — with per-user budgets,
smart routing, and spend tracking that keep the bill small.

</div>

---

## The problem we solve

AI costs add up fast: a plan per person, no visibility into who spent what, and premium prices
paid even for trivial prompts. For a small team, that's hard to justify.

**Axonate fixes the economics:**

- 💸 **Cheap by default** — `auto` routing sends easy/bulk work to the cheapest capable model
  (including **free local models** via Ollama).
- 🛡️ **Hard ceilings** — a global spend cap + per-user budgets that actually block. No surprise bills.
- 📊 **Full visibility** — per-user trace, usage dashboard, and a daily Slack spend digest.
- ☁️ **Use what you already pay for** — route through existing **AWS/Azure** commitments and credits.
- 🔌 **No lock-in** — OpenAI-compatible everywhere; one shared key, every provider, swap freely.

## Projects

| Repo | What |
|---|---|
| 🧠 **[axonate](https://github.com/Axonate/axonate)** | the gateway — routing, budgets, SSO, trace (self-host with Docker) |
| ⌨️ **[ax](https://github.com/Axonate/ax)** | the zero-dependency CLI — `pip install axonate-ax` |
| 🧩 **[vscode](https://github.com/Axonate/vscode)** | VS Code extension — chat with your gateway in the editor |
| 🗺️ **[roadmap](https://github.com/orgs/Axonate/projects/2)** | public board: features, known bugs, planning |
| 📚 **[docs](https://github.com/Axonate/docs)** | guides for CLI, web/API, and IDE setup |

## Use it your way

```bash
# CLI
pip install axonate-ax
ax "summarize this PR"

# Web / any OpenAI-compatible client
curl $AXONATE_URL/v1/chat/completions -H "Authorization: Bearer $KEY" \
  -d '{"model":"auto","messages":[{"role":"user","content":"hi"}]}'

# IDE — VS Code extension, or point Cursor/Continue/Zed at the gateway URL + key
```

## Get started
Stand up the gateway in ~10 minutes → **[Axonate/docs · getting-started](https://github.com/Axonate/docs/blob/main/getting-started.md)**

<div align="center">

---

Built by [CloudDrove](https://clouddrove.com) · MIT licensed

</div>
