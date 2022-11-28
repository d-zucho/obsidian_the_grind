---
<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    await tp.file.rename(title);
  } 
  let book = await tp.system.prompt("Book Name: ")
  let language = await tp.system.prompt("Language: ")
  
  
%>
title:  <% title %>
aliases:
book: <% book %>
language: <% language %>
tags:

---
back:: [[<%tp.file.folder()%>]]