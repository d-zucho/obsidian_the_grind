---


type: codingNote
language: css
topic: @supports -- for unsuported CSS
tags: 

---

back:: (relative = true) => {
      const parent = this.config.target_file.parent;
      let folder;
      if (relative) {
        folder = parent.path;
      } else {
        folder = parent.name;
      }
      return folder;
    }