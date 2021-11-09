## ObjectListener.js

Customizable event listener system for arbitrary objects. It's quite performant
and we use it for state management (see StateManager.js)

```
//Example:
let events = new ObjectListener();
let x = { y: 1, z: { w: 2 }}


events.addListener("y",x,"y");
events.addListener("z",x,"z");

x.z.w = 3;
x.y = 2;
//See console
```


Author: Joshua Brewster
License: AGPL v3.0 License