---
<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    
  } 
	await tp.file.rename(title);
  let language = await tp.system.prompt("Language: ")
  let topic = await tp.system.prompt("Topic: ")

  await tp.file.move("080 - Snippets/" + (await title))
  
%>
title:  <% title %>
alias:
language: <% language %>
topic: <% topic %>
tags: snippets
---

back: [[080 - Snippets]]


## Discription: 





## The Code: 

```

```
