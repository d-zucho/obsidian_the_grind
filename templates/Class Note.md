<%* let title = tp.file.title 
	if (title.startsWith("Untitled")) { 
		title = await tp.system.prompt("Title"); 
		await tp.file.rename(`${title}`); 
		}  
%>



## <% title %>
---
type: classNote
course: 
dateCreated: <% tp.file.creation_date('MMM-Do-YYYY')%>
lastModified: <%tp.file.last_modified_date('MMM-Do-YYYY')%>
title: <% title %>


---

back:: [[<%tp.file.folder()%>]]

