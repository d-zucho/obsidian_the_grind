---
language: css
topic: responsive font-size
---

# Achieving Fluid Typography with `calc`

## Steps:

#### First Step

Think about what you want your **minimum** font-size to be as well as your **largest** font-size.  Basically the range the base size instead of manually entering `16px`




```ad-attention
The formula is basically:
`font-size: calc([min size] + ([maximum size] - [minimum size]) * ((100vw - [minimum viewport width]) / ([maximum viewport width] - [minimum viewport width])));`
```

