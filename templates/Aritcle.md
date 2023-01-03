---

<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    
  } 
	await tp.file.rename(title);
  let language = await tp.system.prompt("Language: ")

  let folder = await tp.system.prompt("Folder :")
  
  let topic = await tp.system.prompt("Topic: ")

	  await tp.file.move("010 - Programming/" + (await folder) + (await title))
  
  
%>
title:  <% title %>
type: codingNote
alias:
topic: <%topic %> 
language: <% language %>
tags: article

---



## Article Name





### Summary

