---

title:  Loading Animation
alias:
language: css
topic: Loading Animation Pure CSS
tags: snippets
---

back: [[080 - Snippets]]


## Discription: 

A pure spinning loading animation made of just CSS



## The Code: 

```CSS

button {
  height: 40px;
  width: 40px;
  background: rgba(0, 0, 0, 0.2);
  border-radius: 50%;
  border: 2px solid rgba(0, 0, 0, 0.4);
  border-top-color: #fff;
  animation: spinner2 600ms linear infinite;

}


@keyframes spinner2 {
    to {
      transform: rotate(360deg);
    }
}

```
