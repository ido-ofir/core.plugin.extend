# core.plugin.extend
Allows plugins to declaratively extend the core object.

```js
 let core = require('core.skeleton');
 
 core.plugin(
     require('core.plugin.extend')
 );
 
 core.plugin({
     name: 'test',
     extend: {
         ok(){ return '√'; }
     }
 });
 
 core.ok();  // '√'
```
