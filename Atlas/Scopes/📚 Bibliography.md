up:: [[🏠 Home]]
# Articles
```dataview
table  year as Year, title as Title, contribution as contribution
from #source/paper
WHERE !contains(file.name, "paperNote")
sort year DESC
```
# Courses
```dataview
table dates
from #source/course
```

# Web
```dataview
table dates
from #source/web 
```


# Books
```dataview
table dates
from #source/book 
```






