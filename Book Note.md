---
<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    await tp.file.rename(title);
  } 
  
  let author = await tp.system.prompt("Author: ")
  let chapter = await tp.system.prompt("Chapter: ")
  let topic = await tp.system.prompt("topic: ")
  let startingDate = await tp.system.prompt("topic: ")
  
%>
type: bookNote
title: <% title %>
chapter: <% chapter %>
topic: <% topic %>
startingDate: <% startingDate %>
Book: book

---
back:: [[<%tp.file.folder()%>]]

**Book Index:** [[<% title %>]]


## Info  

|  --  | --  |  
| --------- | ------ |  
| Author | <% author %> |  
| Date Started | <% dateStarted %> |  
| Topic | <% topic%> |  

---
---




## Chapte Notes


