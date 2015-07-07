SparseArray
======================

Example
```javascript
var SparseArray = require('./sparsearray');

var sa = new SparseArray();
for(var i=0; i<1000000; i+=100) {
    sa.put(i,'hello'+i);
}

console.log(sa.get(300));
console.log(sa.remove(300));
console.log(sa.get(300));
console.log(sa.get(5000));
```