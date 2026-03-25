---
created: 2025-02-19T03:37:12-05:00
tags:
  - linker-exclude
---
collections of facts

---
##### Dynamic References
```dataviewjs
const currentTitle = dv.current().file.name; 
dv.list(dv.pages().where(p => p.file.outlinks.includes(dv.current().file.link)).file.link);
```
---
