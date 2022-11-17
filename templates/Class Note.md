---
<%* let title = tp.file.title 
	if (title.startsWith("Untitled")) { 
		title = await tp.system.prompt("Title"); 
		await tp.file.rename(`${title}`); 
		}  
type: classNote
course: 
%>
---
back:: [[<%tp.file.folder()%>]]