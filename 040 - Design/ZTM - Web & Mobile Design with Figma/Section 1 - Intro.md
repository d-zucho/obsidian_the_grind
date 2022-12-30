---
type: sectionIndex
alias: ["1 - Intro"]
topic: Section 1 Index
course: ztm-web-design
section: 1-Intro
---

```button
name New Intro Note
type note(Untitled) template
action Design Note
color blue
```


```dataview
table topic as "Topic", course as "Course", file.cday as "Created" 
FROM "040 - Design"
where course = "ztm-web-design" and type != "sectionIndex"
and type != "class"
sort file.cday desc
```
