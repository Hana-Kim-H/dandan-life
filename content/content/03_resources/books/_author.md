
# 저자 Index

```dataview
table title as "제목", author as "저자", year as "출간 연도"
from "content/03_resources/books"
where !contains(file.name, "index") and !contains(file.name, "_author")
sort author asc, year asc
```
