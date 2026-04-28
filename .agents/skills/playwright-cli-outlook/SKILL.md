---
name: playwright-cli-outlook
description: Use Playwright to automate Outlook Web (office.com) to send emails. Use when the user requests sending an email via Outlook, automating email composition, or interacting with Outlook Web UI.
license: MIT
argument-hint: <recipient> <subject> <body>
metadata:
  author: student
  version: 0.0.1
---

# Playwright Outlook Web Email Automation

This skill teaches how to use Playwright to send emails using Outlook Web.

## When to use this skill

Use this skill when the user asks to:
- Send an email via Outlook
- Automate email sending
- Use Outlook Web without API access
- Compose and send messages via browser automation

---

## Preconditions

- User must be logged into Outlook Web manually OR Playwright must reuse a saved session (recommended: persistent context)
- Playwright installed (`npm install playwright` or `pip install playwright` depending on stack)

---

## Core workflow (Playwright)

### 1. Launch browser

Use a persistent context so login is preserved:

```bash
npx playwright codegen https://outlook.office.com
```
