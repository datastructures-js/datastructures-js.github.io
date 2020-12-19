# <a href="https://github.com/datastructures-js">datastructures-js<a/>



## [Queue](https://github.com/datastructures-js/queue)
## [Stack](https://github.com/datastructures-js/stack)
## [Set](https://github.com/datastructures-js/set)
## [Linked List](https://github.com/datastructures-js/linked-list)
## [Heap](https://github.com/datastructures-js/heap)
## [Priority Queue](https://github.com/datastructures-js/priority-queue)
## [Graph](https://github.com/datastructures-js/graph)
## [Binary Search Tree](https://github.com/datastructures-js/binary-search-tree)
## [Trie](https://github.com/datastructures-js/trie)


## install
all data structures:
```sh
npm install --save datastructures-js
```

or individually per usage:
```sh
npm install --save @datastructures-js/stack
```

### extend
There are sometimes domain-specific use cases for data structures that require either a tweak or additional functionality. Data structures here are implemented as a base general purpose classes in ES6. You can always use any of these classes to override or extend the functionality in your own code.

#### Example

```js
const { Graph } = require('@datastructures-js/graph');

class BusStationsGraph extends Graph {
  findShortestPath(srcStationId, destStationId) {
    // benefit from Graph to implement your own code 
  }
}
```

## License
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
