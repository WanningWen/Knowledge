---
created: 2025-01-29T01:11:43-06:00
tags:
  - Obsidian
---
[[Git]]
	- [[Ignoring files between windows and mac]]

[[Auto-linking]]
[[Mood tracker]]

## Dynamic References
```dataviewjs
const currentTitle = dv.current().file.name; 
dv.list(dv.pages().where(p => p.file.outlinks.includes(dv.current().file.link)).file.link);
```
---
