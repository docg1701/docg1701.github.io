---
title: Context7 mcp smarter with hooks
date: 2025-08-16 11:39:00 -03:00
layout: post
---

So, after testing and tweaking heimdall-mcp I thought to myself: "Is it possible to integrate context7 calls in certain moments during development so claude code would be forced to automagically check for up-to-date references?"

And the answer is yes. I told claude code to do it just after we analyzed how heimdall works. So claude did a few iterations, corrected some of its own bugs, refined the implementation by itself and it now works!

As needed heimdall-mcp will save and restore memories.
As needed context7-mcp will be called right before coding or debuggin' and fresh references for libraries and frameworks will be integrated into context.

Hopefully that will help mitigate circular and neverending breakage due to shitty old trainning data. Fingers-crossed!