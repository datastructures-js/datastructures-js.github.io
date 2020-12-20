<table>
  <tr>
    <td><a href="https://github.com/datastructures-js/datastructures-js">datastructures-js</a></td>
    <td><img src="https://img.shields.io/npm/v/datastructures-js.svg"/></td>
    <td><img src="https://img.shields.io/npm/dm/datastructures-js.svg"/></td>
  </tr>
  <tr>
    <td><a href="https://github.com/datastructures-js/stack#datastructures-jsstack">Stack</a></td>
    <td><img src="https://img.shields.io/npm/v/@datastructures-js/stack.svg"/></td>
    <td><img src="https://img.shields.io/npm/dm/@datastructures-js/stack.svg"/></td>
  </tr>
  <tr>
    <td><a href="https://github.com/datastructures-js/queue#datastructures-jsqueue">Queue</a></td>
    <td><img src="https://img.shields.io/npm/v/@datastructures-js/queue.svg"/></td>
    <td><img src="https://img.shields.io/npm/dm/@datastructures-js/queue.svg"/></td>
  </tr>
  <tr>
    <td><a href="https://github.com/datastructures-js/set#datastructures-jsset">Set</a></td>
    <td><img src="https://img.shields.io/npm/v/@datastructures-js/set.svg"/></td>
    <td><img src="https://img.shields.io/npm/dm/@datastructures-js/set.svg"/></td>
  </tr>
  <tr>
    <td><a href="https://github.com/datastructures-js/linked-list#datastrucures-jslinked-list">Linked List</a></td>
    <td><img src="https://img.shields.io/npm/v/@datastructures-js/linked-list.svg"/></td>
    <td><img src="https://img.shields.io/npm/dm/@datastructures-js/linked-list.svg"/></td>
  </tr>
  <tr>
    <td><a href="https://github.com/datastructures-js/heap#datastructures-jsheap">Heap</a></td>
    <td><img src="https://img.shields.io/npm/v/@datastructures-js/heap.svg"/></td>
    <td><img src="https://img.shields.io/npm/dm/@datastructures-js/heap.svg"/></td>
  </tr>
  <tr>
    <td><a href="https://github.com/datastructures-js/priority-queue#datastructures-jspriority-queue">Priority Queue</a></td>
    <td><img src="https://img.shields.io/npm/v/@datastructures-js/priority-queue.svg"/></td>
    <td><img src="https://img.shields.io/npm/dm/@datastructures-js/priority-queue.svg"/></td>
  </tr>
  <tr>
    <td><a href="https://github.com/datastructures-js/graph#datastructures-jsgraph">Graph</a></td>
    <td><img src="https://img.shields.io/npm/v/@datastructures-js/graph.svg"/></td>
    <td><img src="https://img.shields.io/npm/dm/@datastructures-js/graph.svg"/></td>
  </tr>
  <tr>
    <td><a href="https://github.com/datastructures-js/binary-search-tree#datastructures-jsbinary-search-tree">Binary Search Tree</a></td>
    <td><img src="https://img.shields.io/npm/v/@datastructures-js/binary-search-tree.svg"/></td>
    <td><img src="https://img.shields.io/npm/dm/@datastructures-js/binary-search-tree.svg"/></td>
  </tr>
  <tr>
    <td><a href="https://github.com/datastructures-js/trie#datastructures-jstrie">Trie</a></td>
    <td><img src="https://img.shields.io/npm/v/@datastructures-js/trie.svg"/></td>
    <td><img src="https://img.shields.io/npm/dm/@datastructures-js/trie.svg"/></td>
  </tr>
</table>

<br/>

# install
all data structures:
```sh
npm install --save datastructures-js
```

or individually per usage:
```sh
npm install --save @datastructures-js/stack
```

# extend
There are sometimes domain-specific use cases for data structures that require either a tweak or additional functionality. Data structures here are implemented as a base general purpose classes in ES6. You can always use any of these classes to override or extend the functionality in your own code.

## Example

```js
const { Graph } = require('@datastructures-js/graph');

class BusStationsGraph extends Graph {
  findShortestPath(srcStationId, destStationId) {
    // benefit from Graph to implement your own code 
  }
}
```

# License
The MIT License (MIT)

Copyright (c) 2015-present Eyas Ranjous <eyas.ranjous@gmail.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
