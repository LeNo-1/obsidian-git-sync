---
cssclasses:
  - cards
  - cards-cover
tags:
  - Books
  - Table
---

```dataview
TABLE Author, ("![|100](" + Cover + ")") AS "Cover", Topics, Rating, Status
FROM "02 - Areas/Literature/Books"
WHERE Complete
SORT file.name ASC
```

[[Library]]