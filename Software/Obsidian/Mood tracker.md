---
created: 2025-01-29T01:11:28-06:00
tags:
  - Obsidian
---

## Dynamic References
```dataviewjs
const currentTitle = dv.current().file.name; 
dv.list(dv.pages().where(p => p.file.outlinks.includes(dv.current().file.link)).file.link);
```
---
