---
type: videoNote
topic: obsidian
dateCreated: 2022/11/27
tags: obsidian, obsidian/plugins

---
link::  [Youtube Link]([(207) Obsidian Plugins: Templater (Part 2 - File Module) - YouTube](https://www.youtube.com/watch?v=LjdJbknTjm4))



_____

# File Module

### Content

This will get all the present *content* in the file:

```
<% tp.file.content %>
```


## Create New

Creates a new file, based on specified template or content

```
<% tp.file.create_new() %>
```

**Arguements**: 
	- *template* - template you want to use
	- *filename* - what you want filename to be
	- *open_new* - if you want to open the newly created file in new window
	- *folder* - where you want it to be saved. ( default is root )


## Last Modified Date

```
<% tp.file.last_modified_date("YYYY-MM-DD") %>
```


## Title

Gets title of note

```
<% tp.file.title %>
```


## Move

```
<%tp.file.move("Path to move to", "File to move") %>
after the last folder, you can just type whatever you want the file to be called
```