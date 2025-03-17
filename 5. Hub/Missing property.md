---
tags:
  - hub
type: hub
time created: 20-08-2024
last modified: 20-08-2024
---
---
```dataview
LIST
FROM !"Templates" and !"Draft/Need convert" and !"Excalidraw"
WHERE !tags or !type or !time-created or !last-modified
WHERE file.name!= "README"
Sort last-modified DESC
```