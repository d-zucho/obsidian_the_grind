---

<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    
  } 
	await tp.file.rename(title);
 

  await tp.file.move("010 - Programming/012 - JavaScript/" + (await title))
  
%>
title:  <% title %>
type: courseNote
aliases:
course: javascript in detail
language: javascript
section: <% tp.file.cursor(1) %>
tags: js


---
back:: [[<%tp.file.folder()%>]]

back:: [[Javascript in Detail - From Beginner to Advanced]]
