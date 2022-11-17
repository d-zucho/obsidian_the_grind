---
<%* let title = tp.file.title 
	if (title.startsWith("JS - Advanced")) { 
		title = await tp.system.prompt("Title"); 
		await tp.file.rename(`${title}`); 
		}
	let section = await tp.system.prompt('Section: ')
%>

type: courseNote
language: javascript
course: javascript advanced concepts
tags: javascript
section: <% section %>

---

back:: [[Javascript - The Advanced Parts]]