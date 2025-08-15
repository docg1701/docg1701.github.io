---
title: Long term memory fixes old training data
date: 2025-08-14 23:14:00 -03:00
layout: post
---



Claude has a bunch of old data built into it. I've been facing a bunch of recurrent bugs that are very difficult to correct and keep coming back as soon as Claude touches the same files over and over again.

It took a while but I figured out Claude was trying to configure and import stuff with complete deprecated syntax. That's because it was trained with up to 18-month deprecated documentation.

Using Context7 mcp I managed to make Claude Opus fix the code and then write down in fine detail what was the problem e how it was fixed.

Then I told it to create a LONG-TERM-MEMORY.md file and store in it that solution. Also added code snippets and through explanations.

Then I made it write a SUMMARY in CLAUDE.md so that Sonnet would be able to fight its will to write bad code in the near future.

Now, whenever the code agent faces an opportunity to bring that bug back to the codebase it will remember that its training is too old to be used and will be directed to the memory file. 

That will (hopefully) keep old bugs from getting back to the system.

BTW, the current bugs that have fixes in my memory file are related to Alembic, SQLModel, PostgreSQL and datetime.now(UTC).