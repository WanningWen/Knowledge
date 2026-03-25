---
created: 2025-01-29T01:11:18-06:00
tags:
  - git
  - Obsidian
---
[[Ignoring files between windows and mac]]

## Dynamic References
```dataviewjs
const currentTitle = dv.current().file.name; 
dv.list(dv.pages().where(p => p.file.outlinks.includes(dv.current().file.link)).file.link);
```
---
