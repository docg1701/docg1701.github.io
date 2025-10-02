---
title: Well, claude is too dumb to code.
date: 2025-10-02 08:28:00 -03:00
layout: post
---

Until early last week I was living the struggle of everyday battles with claude sonnet 4.0 to make it code python, javascript and shell. 
I ran a bunch of PRDs with proper setups for about 3 months and it was so frustrating. No matter how much I'd simplify the task, break down problems or even interfere directly with code, it would eventually run into walls.
The motive for such wall popping up ever so frequently soon became very clear: claude sonnet can't code... no LLM can code. LLMs excel in writing text that resembles code and they get really near to making it work as proper code, but fail when you need it the most: the real world.
So, no matter how much tokens I'd spend, no matter how many hours I'd put into making it write proper code, I would never get to a point where my project (planned and documented by me and written by claude sonnet) would be ready for deployment or real-world use cases.
I gave up for a few days, tried out GLM 4.5 and got a few better results but nothing fancy.
Then claude sonnet 4.5 came about and even GLM 4.6 and i bumped into this idea. Not new, just revisiting. What if i could use claude to build a very thought-out plataform for low-code and no-code development? Maybe n8n, pgvector+postgres, some reverse proxy feature, maybe a login/authentication solution and some sort of frontend development thingie that would make it possible to give a bunch of n8n workflows a proper interface.
I mean, I could deploy that solution to a cheap VPS, build my workflows by hand (or claude/glm-assisted) and sell that with a cute and professional-looking UX.
Is that even possible with opensource?

That is something I would put hours into to validate... stay tuned!