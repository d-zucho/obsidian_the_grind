---
<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    await tp.file.rename(title);
  } 
  let book = await tp.system.prompt("Book Name: ")
  let language = await tp.system.prompt("Language: ")
  let chapter = await tp.system.prompt("Chapter: ")
  let topic = await tp.system.prompt("topic: ")
  
  
%>
type: bookNote
book: <% book %>
title:  <% title %>
chapter: <% chapter %>
topic: <% topic %>
language: <% language %>
tags:

---
back:: [[<%tp.file.folder()%>]]