---
layout: default
permalink: /stack
---

# Stack
<div class="ds-badges">
  <img src="https://img.shields.io/npm/v/@datastructures-js/stack.svg"/>
  <img src="https://img.shields.io/npm/dm/@datastructures-js/stack.svg"/>
</div>
<hr />

## Install
```sh
npm install --save @datastructures-js/stack
```

## require
```js
const { Stack } = require('@datastructures-js/stack');
```

## import
```js
import { Stack } from '@datastructures-js/stack';
```

## Full API
<a href="https://github.com/datastructures-js/stack#table-of-contents">datastructures-js/stack</a>
<br /><br />
## Problems

<p class="problem">Balanced Brackets</p>

{% raw %}
```js
// check if a string has balanced brackets

const Stack = require('@datastructures-js/stack');

function hasBalancedBrackets(str) {
  const leftBrackets = new Set(['(', '[', '{', '<']);

  const rightBrackets = new Map([
    [')', '('],
    [']', '['],
    ['}', '{'],
    ['>', '<']
  ]);

  const stack = new Stack();

  for (let i = 0; i < str.length; i += 1) {
    const char = str[i];
    if (leftBrackets.has(char)) {
      stack.push(char);
    } else if (rightBrackets.has(char)) {
      const matchingLeftBracket = rightBrackets.get(char);
      const topBracket = stack.peek();
      if (matchingLeftBracket === topBracket) {
        stack.pop();
      } else {
        return false;
      }
    }
  }

  return stack.isEmpty();
}

console.log(hasBalancedBrackets('{{<[[<()>]]>}}')); // true
console.log(hasBalancedBrackets('{[()]}}')); // false
```
{% endraw %}
