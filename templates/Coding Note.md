---
<%* let title = await tp.system.prompt("Title"); 
	await tp.file.rename(tp.system.prompt("title"))
		
let language = await tp.system.prompt('language: ');
let topic = await tp.system.prompt('topic: ');

%>

type: codingNote
language: <% language %>
topic: <% topic %>
tags: <% language %>

---
back: [[<% folder %>]]

<% title %>



