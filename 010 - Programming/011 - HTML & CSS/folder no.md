---


type: codingNote
language: css
topic: css test
tags: 

---

back:: (relative = false) => {
      const parent = this.config.target_file.parent;
      let folder;
      if (relative) {
        folder = parent.path;
      } else {
        folder = parent.name;
      }
      return folder;
    }