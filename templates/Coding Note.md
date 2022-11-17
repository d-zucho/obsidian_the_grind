---
<%* 
//	if (tp.file.title == "Untitled") {
		let title = await tp.system.prompt("Title"); 
		tp.file.rename(tp.file.title)
//	}
		
		
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




