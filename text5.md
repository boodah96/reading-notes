# Linked List

a linked list is a linear collection of data elements whose order is not given by their physical placement in memory. Instead, each element points to the next.

### TERMS

- A node is a basic unit of a data structure, such as a linked list or tree data structure. Nodes contain data and also may link to other nodes. Links between nodes are often implemented by pointers.

- Linked List: A data structure that contains nodes that links/points to the next node in the list.

- Singly: Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.

- Doubly: Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.

- Node: Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.

- Next: Each node contains a property called Next. This property contains the reference to the next node.

- Head: The Head is a reference of type Node to the first node in a linked list.

- Current: The Current is a reference of type Node to the node that is currently being looked at. When traversing, you create a new Current variable at the Head to guarantee you are starting from the beginning of the linked list.


**Linked lists are among the simplest and most common data structures. They can be used to implement several other common abstract data types, including lists, stacks, queues, associative arrays, and S-expressions, though it is not uncommon to implement those data structures directly without using a linked list as the basis.**

##### REFRENCES
- https://en.wikipedia.org/wiki/Linked_list
- https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d