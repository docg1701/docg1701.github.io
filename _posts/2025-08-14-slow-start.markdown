---
title: Slow start
date: 2025-08-14 11:41:00 -03:00
---

It's been a slow start, i'v ran 3 ou 4 cycles of the BMAD method and stopped short before completion. It seems claude code, no matter what i try, keeps going back to outdated training data on code syntax. It sux and brakes everything.
On the past week or so I think I found a solution: to develop an intrinsic test script suite that uses proper syntax and is well documented in CLAUDE.md.
I've managed to work around old training data with Context7 MCP to fix a bunch of terrible Vitest config errors.
Also, running claude code in plan mode with Opus 4.1 and Sonnet for writing code itself is the way to go. I still have to watch it and manually accept edits, but it's much better now and crazy dependency cycles are much less common.
As of today, I'll just fix some broken tests there keep showing up and do some more real world testing of the test scripts. Then, back to code development and testing.