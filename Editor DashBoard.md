---
publish: false
---
# In Progress
```dataview
TABLE title, aliases, status
WHERE 
status = "In Progress" OR 
status = "Investigating" OR
status = "Writing"
```


# Backlog
```dataview
TABLE title, aliases
WHERE status = "Backlog" OR status = null
```
