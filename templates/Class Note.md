---
<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    await tp.file.rename(title);
  } 
  let course = await tp.system.prompt("Course Name: ")
  let language = await tp.system.prompt("Language: ")
  
  
%>
title:  <% title %>
aliases:
course: <% course %>
language: <% language %>
tags:

---
back:: [[<%tp.file.folder()%>]]