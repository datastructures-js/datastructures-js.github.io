---
layout: default
permalink: /linked-list
---

# Linked List

<div class="ds-badges">
  <img src="https://img.shields.io/npm/v/@datastructures-js/linked-list.svg"/>
  <img src="https://img.shields.io/npm/dm/@datastructures-js/linked-list.svg"/>
</div>
<hr />

## Problems
<div class="problems">
  <div><a href="#reverse-linked-list">Reverse Linked List</a></div>
  <div><a href="#reverse-doubly-linked-list">Reverse Doubly Linked List</a></div>
</div>
<br/>

## Install
```sh
npm install --save @datastructures-js/linked-list
```

## require
```js
const {
  LinkedList,
  DoublyLinkedList
} = require('@datastructures-js/linked-list');

// list node classes are also exported
const {
  LinkedListNode,
  DoublyLinkedListNode
} = require('@datastructures-js/linked-list');
```

## import
```js
import {
  LinkedList,
  DoublyLinkedList
} from '@datastructures-js/linked-list';

// list node classes are also exported
import {
  LinkedListNode,
  DoublyLinkedListNode
} from '@datastructures-js/linked-list';
```

## Full API
<a href="https://github.com/datastructures-js/linked-list#table-of-contents">datastructures-js/linked-list</a>
<br /><br />
## Problems

<p id="reverse-linked-list" class="problem">Reverse Linked List</p>

{% raw %}
```js
// simple form of linked list is used (object literal)

function reverseLinkedList(currentNode = { next: null }) {
  if (currentNode.next === null) return currentNode;

  const reversed = reverseLinkedList(currentNode.next);
  currentNode.next.next = currentNode;
  currentNode.next = null;

  return reversed;
}

// test

const linkedList = {
  value: 10,
  next: {
    value: 20,
    next: {
      value: 30,
      next: null
    }
  }
};

console.log(reverseLinkedList(linkedList));

/*
{
  value: 30,
  next: {
    value: 20,
    next: {
      value: 10,
      next: null
    }
  }
}
*/
```
{% endraw %}

<p id="reverse-doubly-linked-list" class="problem problem-separator">Reverse Doubly Linked List</p>

{% raw %}
```js
// simple form of doubly linked list is used (object literal)

function reverseDoublyLinkedList(currentNode = { next: null, prev: null }) {
  if (currentNode.next === null) {
    currentNode.prev = null;
    return currentNode;
  }

  const reversed = reverseDoublyLinkedList(currentNode.next);
  currentNode.next.next = currentNode;
  currentNode.prev = currentNode.next;
  currentNode.next = null;

  return reversed;
}

// test

const doublyLinkedList = {
  value: 10,
  prev: null
};
doublyLinkedList.next = {
  value: 20,
  prev: doublyLinkedList
};
doublyLinkedList.next.next = {
  value: 30,
  prev: doublyLinkedList.next,
  next: null
};

/*
<ref *1> {
  value: 10,
  prev: null,
  next: <ref *2> {
    value: 20,
    prev: [Circular *1],
    next: { value: 30, prev: [Circular *2], next: null }
  }
}
*/

console.log(reverseDoublyLinkedList(doublyLinkedList));

/*
<ref *1> {
  value: 30,
  prev: null,
  next: <ref *2> {
    value: 20,
    prev: [Circular *1],
    next: { value: 10, prev: [Circular *2], next: null }
  }
}
*/
```
{% endraw %}
