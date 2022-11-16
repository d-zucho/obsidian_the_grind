---
<%* let title = await tp.system.prompt("Title"); 
		
		
let language = await tp.system.prompt('language: ');
let topic = await tp.system.prompt('topic: ');
let folder = await tp.file.folder(true);
%>

type: codingNote
language: <% language %>
topic: <% topic %>
tags: <% language %>

---
back: [[<% folder %>]]




