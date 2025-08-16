---
title: Long-term memory with heimdall-mcp
date: 2025-08-16 11:31:00 -03:00
layout: post
---

After digging and digging through mcp sludge all over the web I finally found [heimdall](https://github.com/lcbcFoo/heimdall-mcp-server) which actually works.

It integrates with claude code after a fairly quick and easy install and will automagically save memories and recall them as needed. I can talk to claude and make it save or remember or even delete certain memories which is really neat and helpful.

Claude's context windows is quite narrow for long coding sessions, so when it is nearly full, I use heimdall to save a memory and recall it after /clear. Also, I keep memories to be recalled later on to address certain missing features and needed fixes I know I'll forget about.

Be aware that the qdrant docker will be marked is "unhealthy" due to some misconfiguration but it will work fine, just ignore it.

Ah, and of course, I used pipx to install it locally because it is recommended to pip install it as root and Mint linux doesn't like that (and neither do I).