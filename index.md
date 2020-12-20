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
You can always use any of these classes to override or extend the functionality in your own code.

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
The MIT License (MIT). Copyright (c) 2015-present Eyas Ranjous <eyas.ranjous@gmail.com>
