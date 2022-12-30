---

<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    
  } 
	await tp.file.rename(title);
  let section = await tp.system.prompt("Section: ")

  await tp.file.move("040 - Design/ZTM - Web & Mobile Design with Figma/" + (await title))
  
%>
type: sectionIndex
title:  <% title %>
aliases: "ztm-web-design"
course: ztm-web-design
language: design
section: <% section %>
tags: design


---
back:: [[<%tp.file.folder()%>]]




---



```button
name New Section Note
type note(Untitled) template
action Design Note
color blue
```

***** Change DATAVIEW FILTER TO MATCH THIS SECTION*** 
## Section Notes
```dataview
table topic as "Topic", course as "Course", file.cday as "Created" 
FROM "040 - Design"
where course = "ztm-web-design" and type != "sectionIndex"
and type != "class" and section = "2 - Sketching"
sort file.cday desc
```





## Section Resources