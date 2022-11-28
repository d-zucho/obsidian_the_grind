---

<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    await tp.file.rename(title);
    await tp.file.functions.move("010 - Programming/012 - JavaScript/" + tp.file.title)
  } 

  let language = await tp.system.prompt("Language: ")

  
  
%>
title:  <% title %>
aliases:
course: javascript advanced concepts
language: <% language %>
tags: js

---
back:: [[<%tp.file.folder()%>]]

back:: [[Javascript - The Advanced Parts]]