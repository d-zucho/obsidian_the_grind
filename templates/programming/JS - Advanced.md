---
<%* let title = tp.file.title 
	if (title.startsWith("Untitled")) { 
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