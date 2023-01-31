---

<%*
  let title = tp.file.title
  if (title) {
    title = await tp.system.prompt("Title");
    course = await tp.system.prompt("Class: ")
    
  } 
	await tp.file.rename(title);
 

  await tp.file.move("010 - Programming/016 - Python/" + (await title))
  
%>
title:  <% title %>
type: courseNote
aliases:
course: <% course %>
language: python
tags: python


---
back:: [[<%tp.file.folder()%>]]


