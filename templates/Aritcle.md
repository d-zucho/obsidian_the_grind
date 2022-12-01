---

<%*
  let title = tp.file.title
  if (title.startsWith("Untitled")) {
    title = await tp.system.prompt("Title");
    await tp.file.rename(title);
  } 

  let language = await tp.system.prompt("Language: ")
  let topic = await tp.system.prompt("Topic: ")
  
  
%>
title:  <% title %>
type: codingNote
alias:
topic: <%topic %> 
language: <% language %>
tags: article

---

```dataviewjs
	let pg = dv.current() // set pg to be current page
	dv.header(1, pg.title) // title as metadata title
	dv.header(2, "Article" // set topic as h2
```


## Article Name





### Summary

