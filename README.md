glb
===

Empty module, useful for sharing globals across your sub-modules.

# Install

```bash
npm install glb
```

# Example :

- main.js :

```javascript
var glb  = require('glb');
var test = require('./test');

console.log(glb);
```

- test.js :

```javascript
var glb = require('glb');

glb.foo = 42;
```

- output :

```
> node main.js
{ foo: 42 }
```
