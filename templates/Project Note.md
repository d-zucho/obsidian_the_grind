
---
<%* 

	//title.startsWith("Untitled")
		let title = await tp.system.prompt("Title"); 
		await tp.file.rename(`${title}`); 
		let language = await tp.system.prompt("language: ");
		


let title = tp.system.prompt("Note Title: ")
 
%>
type: project
dateCreated: <% tp.file.creation_date('MMM-Do-YYYY')%>
lastModified: <% tp.file.last_modified_date('MMM-Do-YYYY')%>
title: <% await title %>
language: <%  await language %>
tags: project
---



# <%+ title %>





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
 





