---
created: 2025-01-30T19:09:30-06:00
tags:
  - Software/Obsidian/Code
---
`<iframe src="INSERT YOUR URL HERE"></iframe>`
## Embed a YouTube video 

To embed a YouTube video, use the same Markdown syntax as [external images](https://help.obsidian.md/Editing+and+formatting/Basic+formatting+syntax#External%20images):

```md
![](https://www.youtube.com/watch?v=NnTvZWp5Q7o)
```


---
##### Dynamic References
```dataviewjs
const currentTitle = dv.current().file.name; 
dv.list(dv.pages().where(p => p.file.outlinks.includes(dv.current().file.link)).file.link);
```
---
