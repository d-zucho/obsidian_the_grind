---

<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    
  } 
	await tp.file.rename(title);
  let language = await tp.system.prompt("Language: ")

  await tp.file.move("010 - Programming/012 - JavaScript/" + (await title))
  
%>
title:  <% title %>
aliases:
course: javascript advanced concepts
language: <% language %>
section: <% tp.file.cursor(1) %>
tags: js


---
back:: [[<%tp.file.folder()%>]]

back:: [[Javascript - The Advanced Parts]]
