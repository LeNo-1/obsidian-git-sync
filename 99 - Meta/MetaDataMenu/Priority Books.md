---
cssclasses:
  - cards
---

```dataview
TABLE Author, ("![|100](" + Cover + ")") AS "Cover", Topics, Rating, Status
FROM "02 - Areas/Literature/Books"
WHERE Priotity
SORT file.name ASC
```