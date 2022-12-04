---

<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    
  } 
	await tp.file.rename(title);
	
  await tp.file.move("040 - Design/" + (await title))
  
%>
title:  <% title %>
type: designNote
alias: ["ztm-web-design"]
course: ztm-web-design
section: <% tp.file.cursor(1) %>
tags: 


---
back: [[<%tp.file.folder()%>]]