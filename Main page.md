# 🏠 Project Name: 

# Short summary

## Project info
- **PI/ Group:** 
- **Main contact:** 
- **Start date:** 
- **Redmine issue:** 

## External links
- [Confluence space](https://)
- [Github repository](https://)
- [Google notes](https://)
- [Redmine issue page](https://)

## Monthly summaries
```dataview
LIST
FROM "Monthly"
SORT file.name DESC
```

## Recent meetings
```dataview
LIST
FROM "Meetings"
SORT file.day DESC
LIMIT 10
```

## Recent daily notes
```dataview
LIST
FROM "Daily"
SORT file.name DESC
LIMIT 7
```

## Open tasks
```dataview
TASK
FROM "Daily" OR "Meetings"
WHERE !completed
GROUP BY file.link
SORT file.day DESC
```

## Other documents
- 
