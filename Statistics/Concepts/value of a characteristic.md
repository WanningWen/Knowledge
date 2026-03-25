---
created: 2025-02-19T03:41:23-05:00
tags:
  - Statistics
---
- a category (e.g., female or insufficient solder)
- a number (e.g., age5 23 years or diameter5 .502 cm)

---
##### Dynamic References
```dataviewjs
const currentTitle = dv.current().file.name; 
dv.list(dv.pages().where(p => p.file.outlinks.includes(dv.current().file.link)).file.link);
```
---
