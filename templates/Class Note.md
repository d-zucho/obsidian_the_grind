<%* let title = tp.file.title 
	if (title.startsWith("Class Note")) { 
		title = await tp.system.prompt("Title"); 
		await tp.file.rename(`${title}`); 
		}  
type: classNote
course: 






dateCreated: <% tp.file.creation_date('MMM-Do-YYYY')%>
lastModified: <%tp.file.last_modified_date('MMM-Do-YYYY')


---

back:: [[<%tp.file.folder()%>]]

