---
<%* let title = tp.file.title 
		title = await tp.system.prompt("Title"); 
		await tp.file.rename(`${title}`); 
		
	let language = await tp.system.prompt('language: ')
	let topic = await tp.system.prompt('topic: ')
	let folder = await tp.file.folder(true)
%>

type: codingNote
language: <% language %>
topic: <% topic %>
tags: 

---
<% folder %>

back:: <% tp.file.folder %>


# <% title %>
