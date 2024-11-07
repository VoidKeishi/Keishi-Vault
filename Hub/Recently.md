---
tags:
  - hub
type:
  - hub
time created: 19-08-2024
last modified: 19-08-2024
---

```dataview
TABLE last-modified AS "Last modified"
FROM !"Templates"
WHERE last-modified 
Sort last-modified DESC
Limit 25
```