# Data Structures

## 2. Linked Lists

### Description
A linked list is a linear data structure where each element, called a node, contains a reference (or link) to the next node in the sequence. Unlike arrays, linked lists do not require a contiguous block of memory, which allows for efficient insertion and deletion of elements. Each node typically contains two parts:
- **Data**: The value or information stored in the node.
- **Pointer**: A reference to the next node in the list.

### Types
- **Singly Linked List**: In a singly linked list, each node has a single pointer that points to the next node. This allows for traversal of the list in one direction, from the head to the end.

  **Example**:
Head -> Node1 -> Node2 -> Node3 -> NULL

- **Doubly Linked List**: In a doubly linked list, each node has two pointers: one pointing to the next node and one pointing to the previous node. This allows for bidirectional traversal of the list, making operations such as insertion and deletion more flexible.

**Example**:
NULL <- Head <-> Node1 <-> Node2 <-> Node3 -> NULL

### Use Cases
- **Dynamic Data Storage**: Linked lists are ideal for scenarios where the number of elements is not known in advance or changes frequently. They are used in applications where elements are frequently inserted or removed, such as in a queue or stack implementation.
- **Memory Efficiency**: Linked lists can efficiently use memory for large datasets or systems with fragmented memory, as they do not require contiguous memory allocation.
- **Implementing Data Structures**: Linked lists serve as the foundation for other complex data structures such as hash tables, graphs, and more advanced list-based data structures.

### Pros
- **Dynamic Size**: Linked lists can grow or shrink in size dynamically, as nodes are allocated and deallocated as needed. This flexibility makes them suitable for scenarios with varying data sizes.
- **Efficient Insertions/Deletions**: Inserting or deleting nodes in a linked list is generally more efficient compared to arrays, especially when performed at the beginning or middle of the list. These operations can be done in O(1) time if the node reference is known.

### Cons
- **Slower Access Time**: Accessing an element in a linked list requires traversal from the head node, which can be slower compared to arrays where elements can be accessed directly by index. The time complexity for accessing an element is O(n) in the worst case.
- **Extra Memory for Pointers**: Each node in a linked list requires additional memory for storing pointers (or references) to other nodes. This overhead can increase the memory usage compared to arrays, where only the data itself is stored.
- **Complex Implementation**: Linked lists can be more complex to implement and manage compared to arrays, as they require careful handling of node pointers to avoid issues such as memory leaks or broken links.

### Example
Here's a simple example of a singly linked list implementation in JavaScript:

```javascript
class Node {
  constructor(data) {
      this.data = data;
      this.next = null;
  }
}

class LinkedList {
  constructor() {
      this.head = null;
  }

  // Add a node to the end of the list
  append(data) {
      const newNode = new Node(data);
      if (this.head === null) {
          this.head = newNode;
          return;
      }

      let current = this.head;
      while (current.next !== null) {
          current = current.next;
      }
      current.next = newNode;
  }

  // Display the list
  display() {
      let current = this.head;
      while (current !== null) {
          console.log(current.data);
          current = current.next;
      }
  }
}

// Usage
const list = new LinkedList();
list.append(1);
list.append(2);
list.append(3);
list.display(); // Output: 1, 2, 3
```
