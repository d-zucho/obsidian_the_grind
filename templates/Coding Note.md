---
<%* let title = tp.file.title 
	if (title.startsWith("Untitled")) { 
		title = await tp.system.prompt("Title"); 
		await tp.file.rename(`${title}`); 
		}
	let language = await tp.system.prompt('language: ')
	let topic = await tp.system.prompt('topic: ')
%>

type: codingNote
language: <% language %>
topic: <% topic %>
tags: 

---

back:: <% tp.file.folder %>