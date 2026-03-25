---
created: 2025-02-19T03:38:29-05:00 
tags:
  - your-default-tags
---
When desired information is available for all objects in the population

---
##### Dynamic References
```dataviewjs
const currentTitle = dv.current().file.name; 
dv.list(dv.pages().where(p => p.file.outlinks.includes(dv.current().file.link)).file.link);
```
---
