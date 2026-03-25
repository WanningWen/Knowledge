---
created: 2025-01-29T13:42:25-06:00
tags:
  - Software/Obsidian
---
https://github.com/mgmeyers/obsidian-style-settings


---
##### Dynamic References
```dataviewjs
const currentTitle = dv.current().file.name; 
dv.list(dv.pages().where(p => p.file.outlinks.includes(dv.current().file.link)).file.link);
```
---
