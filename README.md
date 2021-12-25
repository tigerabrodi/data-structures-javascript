# Map

- Map is like an object, but the main difference is that it allows keys of any type.

- Methods, set, get, has, delete, clear, size

- Looping over a map: keys, values or entries.

- Map has a forEach method built-in.

- Init a map with an array of key value pairs: `new Map([['1',  'str1'], [1,    'num1'], [true, 'bool1']])`

- To turn an object into a Map, we can use `Object.entries`, which returns an array of key/value pairs: `const map = new Map(Object.entries(obj));`.

- Object.fromEntries, given an array of key/value paires, creates an object from it, we can use it to turn a Map into an object. `const obj = Object.fromEntries(map.entries()/map);`.


# Set

- Set of values, no keys, where each value may only exist once, unique.

- Create via `new Set()`.

- Methods: add, delete, has, clear, size

- Only works with values.


# WeakMap

- By default the JavaScript engine keeps a value in memory while it is "reachable" and can potentially be used.

- WeakMap is fundamentally different, it doesn't prevent garbage-collection of key objects.

- Keys must be objects.

- If there are no other references to an object, it will be removed from memory (and automatically from the WeakMap).

- Methods: get, set, delete, has

- Great for usecases where cleaning up is important, i.e. caching.


# WeakSet

- Only add objects.


With WeakMap and WeakSet, the weakness is the iterations to get all the objects.
