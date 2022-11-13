---
<%* let title = tp.file.title 
	if (title.startsWith("Untitled")) { 
		title = await tp.system.prompt("Title"); 
		await tp.file.rename(`${title}`); 
		}
	let language = await tp.system.prompt('language: ')
	let instructor = await tp.system.prompt('instructor/s: ')
%>

title: <% title %>
alias: <% tp.file.cursor(1) %>
language: <% language %>
tags: <% tp.file.cursor(2) %>
dateStarted: <% tp.file.creation_date("MMM Do YYYY") %>
---

back::  <% tp.file.folder() %>

___


## Class Index




### 📜 Notes and Ideas

-   first Note



### 🔗 Github Project Links




### 📦 Resources
