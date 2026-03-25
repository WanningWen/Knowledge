---
created: 2025-02-05T13:41:45-06:00
tags:
  - Nonprofit/Org
---
https://unheardvoicesoutreach.org/

---
##### Dynamic References
```dataviewjs
const currentTitle = dv.current().file.name; 
dv.list(dv.pages().where(p => p.file.outlinks.includes(dv.current().file.link)).file.link);
```
---
