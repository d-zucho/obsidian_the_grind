---

<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    await tp.file.rename(title);
  } 

  let language = await tp.system.prompt("Language: ")
  let topic = await tp.system.prompt("Topic: ")
  let folder = await tp.system.suggester("What folder?", "012 - JavaScript")
  
  
%>
title:  <% title %>
type: codingNote
alias:
topic: <%topic %> 
language: <% language %>
tags: 

---
back:: [[<%tp.file.folder()%>]]


