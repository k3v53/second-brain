---
publish: false
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