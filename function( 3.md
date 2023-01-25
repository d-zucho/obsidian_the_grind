---

<%*
  let title = tp.file.title
  if (title)) {
    title = await tp.system.prompt("Title: ");
    await tp.file.rename(title);
   
	
  let language = await tp.system.prompt("Language: ")
  let course = await tp.system.prompt("Course: ")
  let teacher = await tp.system.prompt("Teacher: ")
  let topic = await tp.system.prompt("Topic: ")
  
  await tp.file.move("010 - Programming/015 - React/" + (await title))
  }
%>
title:  <% title %>
type: classNote
course: <% course %>
teacher: <% teacher %>
alias:
topic: <%topic %> 
language: <% language %>
tags: 

---
back: <% tp.file.folder() %>