
---
<%* 

  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    await tp.file.rename(title);
  } 

  let language = await tp.system.prompt("Language: ")


 
%>
type: project
dateCreated: <% tp.file.creation_date('MMM-Do-YYYY')%>
title: <% title %>
language: <% language %>
tags: project
---
lastModified::  <% tp.file.last_modified_date('MMM-Do-YYYY')%>


# <% tp.file.title %>





## Details

#### Tech Stack: 

-  tech 1
-  tech 2


**Desired Outcome** / **Purpose / Intention **

-  What is this for? 


_________

### Next Actions

- [ ]  Rough Design
- [ ] Do I need Figma Design Ready?
 





