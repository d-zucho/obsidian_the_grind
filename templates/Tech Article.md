---

<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    
  } 
  let type = await tp.system.prompt("Type: ")
	
  let language = await tp.system.prompt("Language: ")

  await tp.file.rename(title);
  await tp.file.move("070 - Random/073 - Technology/" + (await title))
  
%>
title:  <% title %>
type: "tech-article"
aliases:
course: javascript advanced concepts
language: <% language %>
section: <% tp.file.cursor(1) %>
tags: 
---
back:: [[<%tp.file.folder()%>]]



## Article Name





### Summary

