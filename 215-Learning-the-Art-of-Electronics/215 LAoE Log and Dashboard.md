---
publish: false
---

## Inbox
```dataview
table status
where contains(file.tags, "#inbox") and contains(file.path, this.file.folder)
```

> [!TIP]- Anki Todo
> 
> ```query
> tag:#anki-todo
> path:200-Courses/215-LAoE
> ```

> [!TIP]- Images Todo
> ```query
> tag:#todo/img
> path:200-Courses/215-LAoE
> ```

> [!TIP]- Questions Todo
> ```query
> tag:#q
> path:200-Courses/215-LAoE
> ```

## Class Notes
```dataview
table status, Summary
where contains(file.folder, this.file.folder) and !contains(file.name, "_")
sort file.name asc
```


## Garden Notes
```dataview
table status, class, file.tags
from #t/analog 
where !contains(file.tags, "#example")
sort file.mtime DESC
```