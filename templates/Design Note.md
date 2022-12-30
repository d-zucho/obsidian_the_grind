---

<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    
    
  } 
	await tp.file.rename(title);
	let section = await tp.system.prompt("Section: ")
	
	await tp.file.move("040 - Design/" + (await title))
%>
title:  <% title %>
type: designNote
alias: ["ztm-web-design"]
course: ztm-web-design
section: <% section %>
topic:
tags: 


---
back: [[<%tp.file.folder()%>]]


