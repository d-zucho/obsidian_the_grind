---
<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    await tp.file.rename(title);
  } 
  let book = await tp.system.prompt("Book Name: ")
  let author = await tp.system.prompt("Author: ")
  let chapter = await tp.system.prompt("Chapter: ")
  let topic = await tp.system.prompt("topic: ")
  let startingDate = tp.file.creation_date("MMM-Do-YYYY")
  
%>
type: bookIndex
book: <% book %>
chapter: <% chapter %>
topic: <% topic %>
startingDate: <% startingDate %>
tags: book

---
back:: [[<%tp.file.folder()%>]]


## Info  

|  --  | --  |  
| --------- | ------ |  
| Author | <% author %> |  
| Date Started | <% dateStarted %> |  
| Topic | <% topic%> |  

---
---



> [!abstract] Summary
> What is this book about? (in own words quick summary)


## Book Notes

Insert dataview here?