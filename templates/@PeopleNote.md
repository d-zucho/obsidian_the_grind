---
<%* let title = tp.file.title 
	if (title.startsWith("@")) { 
		title = await tp.system.prompt("Title"); 
		await tp.file.rename(`${title}`); 
		tp.file.title.slice(1)
		}  
%>
type: project
dateCreated: <% tp.file.creation_date('MMM-Do-YYYY')%>
lastModified: <%tp.file.last_modified_date('MMM-Do-YYYY')%>
title: <% title %>
---