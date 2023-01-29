---

<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    
  } 
  let type = await tp.system.prompt("Type: ")
	
  let subject = await tp.system.prompt("What's the subject? ")

  await tp.file.rename(title);
  await tp.file.move("070 - Random/073 - Technology/" + (await title))
  
%>
title:  <% title %>
type: techArticle
aliases:
subject: <% subject %>
tags: 
---
back:: [[<%tp.file.folder()%>]]



## Article Name





### Summary

