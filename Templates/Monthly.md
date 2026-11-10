[[Main page]]
# Summary: `= this.file.name`

## Completed tasks
```dataview
TASK
FROM "Daily" OR "Meetings"
WHERE completed AND dateformat(file.day, "yyyy-MM") = this.file.name
GROUP BY file.link
```

## Still open
```dataview
TASK
FROM "Daily" OR "Meetings"
WHERE !completed AND dateformat(file.day, "yyyy-MM") = this.file.name
GROUP BY file.link
```

## Meetings this month
```dataview
LIST
FROM "Meetings"
WHERE dateformat(file.day, "yyyy-MM") = this.file.name
SORT file.day ASC
```

## Highlights / manual notes
