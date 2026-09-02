<div align="center">
<h1>claude-session-trigger</h1>
 
[![Claude Session Trigger](https://github.com/Samxel/claude-session-trigger/actions/workflows/claude-session-trigger.yml/badge.svg)](https://github.com/Samxel/claude-session-trigger/actions/workflows/claude-session-trigger.yml)

</div>

This workflow sends one minimal request twice a day on a schedule so the claude usage window opens
at fixed times (ideally before you start working) so you get more out of your claude session.

## Setup

Generate a token on a machine with a browser:

```bash
claude setup-token
```

Copy the `sk-ant-oat01-...` string it prints.

In the repo: **Settings → Secrets and variables → Actions → New repository secret**

| Name | Value |
| --- | --- |
| `CLAUDE_CODE_OAUTH_TOKEN` | the token from above |
---
> [!NOTE]
> Every run consumes real quota from the subscription. It's small (one turn, Haiku,
thinking off) but it isn't free.
