# Security Policy

## Reporting a vulnerability
Please **do not** open a public issue for security problems.

- Use GitHub's **private vulnerability reporting** on the affected repo
  (Security → Report a vulnerability), or
- email **security@clouddrove.com**.

We'll acknowledge within 3 business days and keep you updated through to a fix.

## Scope
Axonate self-hosts an AI gateway. Of particular interest: auth/JWT verification, the CLI
adapter (runs agent CLIs), secret handling, and budget/quota bypass.

## Good to know
- Secrets live only in gitignored `.env` files — never commit them.
- Run the adapter read-only by default; enable write profiles deliberately.
