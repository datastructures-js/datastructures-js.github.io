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

<p class="problem">Reverse Linked List</p>

{% raw %}
```js
// simple form of linked list is used (object literal)

function reverseLinkedList(linkedList) {
  if (linkedList === null) null;
  if (linkedList.next === null) return linkedList;

  const next = reverseLinkedList(linkedList.next);
  linkedList.next.next = linkedList;
  linkedList.next = null;

  return next;
}

const linkedList = {
  value: 10,
  next: {
    value: 20,
    next: {
      value: 30, next: null
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
```
{% endraw %}

