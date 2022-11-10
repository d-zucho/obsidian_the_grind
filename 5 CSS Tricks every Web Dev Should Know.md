---
source: https://www.youtube.com/watch?v=wfaDzSL6ll0
language: css
---






# CSS Tricks

## Background-image and Blend mode


We can have both an image as a background and mix in a color. Almost have effects like those in *photoshop*
Do  this with the following:

```css

body {
	background-image: url(photo.jpg);
	background-color: #00ce2d;
	background-blend-mode: screen;  /* or darken, lighten, or etc.*/
}
```







## Clipping

This makes it possible to put images over certain shapes or specifics on the page:

The html:
```html
<body>
	<div classname='bg'>
		...
		...
	</div>
</body>
```

The CSS:

```css

.bg {
	height: 100%;
	width: 100%;
	background-color: rgb( 2, 211, 248);
	clip-path: polygon(100% 1%, 100% 49%, 49% 99%, 0 99%, 0 0);
	/* You can find these and generate the code online */
	```

#### Some resources to get code:
[Clippy](https://bennettfeely.com/clippy/)


![[Pasted image 20220912154818.png]]


##### Will look something like :
![[Pasted image 20220912155658.png]]

(Without the person image!)
