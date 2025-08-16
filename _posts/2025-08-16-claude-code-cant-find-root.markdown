---
title: Claude code can't find root
date: 2025-08-16 11:45:00 -03:00
layout: post
---

Claude code will eventually lose its track of where it is in the code base. It sux, because it will hallucinate like a crazy bitch on LSD.

So I found out you could set CLAUDE_BASH_MAINTAIN_PROJECT_WORKING_DIR=true in settings.json and it should always get back to the root directory as soon as the tool-call ends. That's sounds great!

So my settings.json in \~/.claude looks like this now:

```bash
{
  "statusLine": {
    "type": "command",
    "command": "bash ~/.claude/statusline-script.sh"
  },
  "model": "opusplan",
  "env": {
    "CLAUDE_BASH_MAINTAIN_PROJECT_WORKING_DIR": "true"
  }
}
```
Will it work? Time will tell.