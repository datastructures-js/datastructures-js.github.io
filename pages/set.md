---
layout: default
permalink: /set
---

# Set
<div class="ds-badges">
  <img src="https://img.shields.io/npm/v/@datastructures-js/set.svg"/>
  <img src="https://img.shields.io/npm/dm/@datastructures-js/set.svg"/>
</div>
<hr />

## Install
```sh
npm install --save @datastructures-js/set
```

## require
```js
const EnhancedSet = require('@datastructures-js/set');
```

## import
```js
import EnhancedSet from '@datastructures-js/set';
```

## API
<a href="https://github.com/datastructures-js/set#api">github.com/datastructures-js/set#api</a>
<br /><br />
## Problems

<p class="problem">First Duplicate</p>

{% raw %}
```js
// find the first duplicate number in an array

function firstDuplicate(arr) {
  const visitedNumbers = new Set();

  for (let i = 0; i < arr.length; i += 1) {
    if (visitedNumbers.has(arr[i])) {
      return arr[i];
    }
    visitedNumbers.add(arr[i]);
  }

  return -1;
}

console.log(firstDuplicate([3,1,2,6,6,2,2,6,7])); // 6
console.log(firstDuplicate([1,2,3,4,5])); // -1
```
{% endraw %}