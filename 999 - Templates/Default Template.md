---
<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    await tp.file.rename(title);
  } 
  
  
%>
title:  <% title %>
dateCreated: <% tp.date.now("dddd Do MMMM YYYY HH:mm") %>
lastModified: <% tp.file.last_modified_date("dddd Do MMMM YYYY HH:mm") %>
Aliases: 
Tags:

---




# <% title %>