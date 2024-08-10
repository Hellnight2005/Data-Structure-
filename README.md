# Data Structures

## 1. Arrays
- **Description**: A collection of elements identified by index or key.
- **Use Cases**: Storing a list of items (e.g., a list of numbers or names).
- **Pros**: Fast access by index.
- **Cons**: Fixed size, inefficient for inserting or deleting elements.

## 2. Linked Lists
- **Description**: A linear collection of elements (nodes), where each node points to the next.
- **Types**:
  - **Singly Linked List**: Each node has a single pointer to the next node.
  - **Doubly Linked List**: Each node has pointers to both the next and previous nodes.
- **Use Cases**: Dynamic data storage where elements are frequently inserted or removed.
- **Pros**: Dynamic size, efficient insertions/deletions.
- **Cons**: Slower access time compared to arrays, extra memory for pointers.

## 3. Stacks
- **Description**: A collection of elements with Last In First Out (LIFO) access.
- **Operations**:
  - **Push**: Add an element.
  - **Pop**: Remove the top element.
- **Use Cases**: Undo mechanisms, function call management.
- **Pros**: Simple operations, efficient for LIFO tasks.
- **Cons**: Limited access (only the top element can be accessed).

## 4. Queues
- **Description**: A collection of elements with First In First Out (FIFO) access.
- **Operations**:
  - **Enqueue**: Add an element.
  - **Dequeue**: Remove the front element.
- **Use Cases**: Task scheduling, buffering.
- **Pros**: Simple operations, efficient for FIFO tasks.
- **Cons**: Limited access (only the front and rear elements can be accessed).

## 5. Hash Tables
- **Description**: A collection of key-value pairs with fast access based on a hash function.
- **Operations**:
  - **Insert**: Add a key-value pair.
  - **Lookup**: Retrieve the value associated with a key.
  - **Delete**: Remove a key-value pair.
- **Use Cases**: Implementing associative arrays, databases.
- **Pros**: Fast average-time complexity for search, insert, and delete operations.
- **Cons**: Potential hash collisions, requires good hash function design.

## 6. Trees
- **Description**: A hierarchical structure consisting of nodes with a root and children.
- **Types**:
  - **Binary Trees**: Each node has up to two children.
  - **Binary Search Trees (BST)**: Left child nodes are less than the parent, right child nodes are greater.
  - **AVL Trees**: Self-balancing BST.
  - **Heap**: A complete binary tree used to implement priority queues.
- **Use Cases**: Hierarchical data representation, efficient searching and sorting.
- **Pros**: Organized structure, efficient search, insert, and delete operations (in balanced trees).
- **Cons**: Can become unbalanced, complexity in implementation.

## 7. Graphs
- **Description**: A collection of nodes (vertices) connected by edges.
- **Types**:
  - **Directed Graphs**: Edges have a direction.
  - **Undirected Graphs**: Edges have no direction.
  - **Weighted Graphs**: Edges have weights.
  - **Unweighted Graphs**: Edges do not have weights.
- **Use Cases**: Network routing, social networks.
- **Pros**: Versatile representation of relationships.
- **Cons**: Can be complex to implement and manage.

## 8. Heaps
- **Description**: A specialized tree-based data structure that satisfies the heap property.
- **Types**:
  - **Min-Heap**: Parent nodes are less than or equal to child nodes.
  - **Max-Heap**: Parent nodes are greater than or equal to child nodes.
- **Use Cases**: Priority queues, heap sort.
- **Pros**: Efficient priority queue operations.
- **Cons**: Less efficient for other operations compared to balanced trees.
