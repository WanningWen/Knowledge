---
created: 2025-02-19T13:46:51-05:00
tags:
  - Statistics
---
a single number that is our “best” guess

---
##### Dynamic References
```dataviewjs
const currentTitle = dv.current().file.name; 
dv.list(dv.pages().where(p => p.file.outlinks.includes(dv.current().file.link)).file.link);
```
---
