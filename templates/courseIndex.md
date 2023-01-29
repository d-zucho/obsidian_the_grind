---
<%* let title = tp.file.title 
	if (title) { 
		title = await tp.system.prompt("Title"); 
		await tp.file.rename(`${title}`); 
		}
	let language = await tp.system.prompt('language: ')
	let teacher = await tp.system.prompt('instructor/s: ')
%>
type: courseIndex
title: <% title %>
alias: 
language: <% language %>
teacher: <% teacher %>
tags: 
dateStarted: <% tp.file.creation_date("MMM Do YYYY") %>
status: open
---

back::  [[<%* tp.file.folder() %>]]

___



## Class Index




### 📜 Notes and Ideas

-   first Note



### 🔗 Github Project Links




### 📦 Resources
