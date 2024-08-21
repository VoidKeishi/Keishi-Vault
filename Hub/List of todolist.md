---
tags:
  - hub
type:
  - hub
time created: 20-08-2024
last modified: 20-08-2024
---
---
```dataview
TABLE last-modified AS "Last modified", tags AS "Tags"
FROM !"Templates"
WHERE contains(tags,"todo") and file.name!=Todolist
Sort last-modified DESC
Limit 25
```
