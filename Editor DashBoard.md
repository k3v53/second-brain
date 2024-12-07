---
draft: true
tags:
  - English
---
# In Progress

```dataview
TABLE aliases, status, file.mtime AS "Modified Date"
WHERE 
status = "In Progress" OR 
status = "Investigating" OR
status = "Writing"
SORT file.mtime DESC
```

# Backlog
```dataview
TABLE aliases, file.mtime AS "Modified Date"
WHERE status = "Backlog" OR status = null
SORT file.mtime DESC
```

# Finished (or closely at least)
```dataview
TABLE aliases, status, file.mtime AS "Modified Date"
WHERE status = "Finished" OR status = "PseudoFinished"
SORT file.mtime DESC
```

> [!info] Statuses
> 1. Finished
> 	1. Finished
> 	2. PseudoFinished
> 2. In Progress
> 	1. Writing
> 	2. Investigating
> 	3. In Progress
> 3. Pending
> 	1. Backlog

> [!note] 
> Is a draft just to hide it from quartz