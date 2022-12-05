---
type: index
tags: snippets


---


# Snippets


```button
name New Snippet
type note(Untitled) template
action New Snippet
color blue
```
## CSS & Styling
```dataview
table language as "Language", topic as "Topic"
from #snippets where type != "index"
where contains(language, "css") OR contains(language, "tailwind")
```


