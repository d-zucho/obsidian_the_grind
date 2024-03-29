---
type: index
language: react
---



## Articles
```dataview
table topic as "Topic"
FROM #article
where language = "react"
```


## Projects
```dataview
table status as "Status", dateCreated as "Date Started" 
FROM #project 
WHERE language = "react" AND status = "active"
```


```button
name New React Course
type note(function(){return this.inputEl.value}) template
action courseIndex
templater true
color blue
```
^button-ubd8


## Courses
![[Courses - React]]



## Notes

```button
name New React Note
type note(Untitled) template
action React Note Template
color blue
```

```dataview
table topic as "Topic"
from #react 
where language = "react"
```


%% Begin Waypoint %%
- [[Buiding Essential UI Data Elements in React]]
- [[Calling from API with fetch()]]
- **[[Courses]]**
- [[Courses - React]]
- [[Dont Use && To Render]]
- [[Flux]]
- [[General Rules of Props]]
- [[handleClick To Delete Item in List]]
- [[Props]]
- [[React Articles]]
- [[React Fundamentals]]
- [[React is Declarative]]
- [[React Refs]]
- [[React State]]
- [[Redux]]
- [[Set Form Input as State]]
- [[useRef Hook]]
- [[Using Context API]]
- [[VirtualDOM]]

%% End Waypoint %%

# React



```ad-summary
title: Ways To Pass Data To/From Components
1. Render Props
2. Context API
3. React Hooks(useContext API)
4. React-Redux / Redux
5. Other state management libraries (i.e. XState, MobX)
```




[[React State]]

### handleClick events to Delete Item in Mapped List

[[handleClick To Delete Item in List]]  :
![[handleClick To Delete Item in List]]



### Set Form Input as State
![[Set Form Input as State]]

## Context API
![[Using Context API]]
