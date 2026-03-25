---
created: 2025-01-29T12:28:20-06:00 
tags:
  - your-default-tags
---
Dependent variable: what you measure

Independent variable: what you vary



---
##### Dynamic References
```dataviewjs
const currentTitle = dv.current().file.name; 
dv.list(dv.pages().where(p => p.file.outlinks.includes(dv.current().file.link)).file.link);
```
---
