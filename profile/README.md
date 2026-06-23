<div align="center">

# Axonate

### One key, every model — shared AI for small teams.

**Stop buying an AI seat for everyone.** Axonate is a self-hosted, OpenAI-compatible gateway
that lets a small company run a few flat AI subscriptions and share them across the whole team —
with per-user budgets, smart routing, and spend tracking that keep the bill small.

</div>

---

## The problem we solve

AI subscriptions and API plans add up fast: one seat per person, no visibility into who spent
what, and premium prices paid even for trivial prompts. For a small team, that's hard to justify.

**Axonate fixes the economics:**

- 🤝 **Share, don't multiply** — one gateway on a couple of subscriptions serves everyone.
- 💸 **Cheap by default** — `auto` routing sends easy/bulk work to the cheapest capable model.
- 🛡️ **Hard ceilings** — a global spend cap + per-user budgets that actually block. No surprise bills.
- 📊 **Full visibility** — per-user trace, usage dashboard, and a daily Slack spend digest.
- 🔌 **No lock-in** — OpenAI-compatible everywhere; grow to real provider APIs with a one-line swap.

## Projects

| Repo | What |
|---|---|
| 🧠 **[axonate](https://github.com/Axonate/axonate)** | the gateway — routing, budgets, SSO, trace (self-host with Docker) |
| ⌨️ **[ax](https://github.com/Axonate/ax)** | the zero-dependency CLI — `pip install axonate-cli` |
| 🧩 **[vscode](https://github.com/Axonate/vscode)** | VS Code extension — chat with your gateway in the editor |
| 📚 **[docs](https://github.com/Axonate/docs)** | guides for CLI, web/API, and IDE setup |

## Use it your way

```bash
# CLI
pip install axonate-cli
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
