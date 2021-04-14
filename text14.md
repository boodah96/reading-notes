## Trees

- a tree is a widely used abstract data type that simulates a hierarchical tree structure, with a root value and subtrees of children with a parent node, represented as a set of linked nodes.

- A tree data structure can be defined recursively as a collection of nodes (starting at a root node), where each node is a data structure consisting of a value, together with a list of references to nodes (the "children"), with the constraints that no reference is duplicated, and none points to the root.

 ## Terms
`Node` - A Tree node is a component which may contain it’s own values, and references to other nodes
`Root` - The root is the node at the beginning of the tree
`K` - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
`Left` - A reference to one child node, in a binary tree
`Right` - A reference to the other child node, in a binary tree
`Edge` - The edge in a tree is the link between a parent and child node
`Leaf` - A leaf is a node that does not have any children
`Height` - The height of a tree is the number of edges from the root to the furthest leaf

#### categories of traversals:
- Depth First:
 - Pre-order:` root >> left >> right`
 - In-order: `left >> root >> right`
 - Post-order: `left >> right >> root`

- Breadth First


### K-ary Trees
If Nodes are able have more than 2 child nodes, we call the tree that contains them a K-ary Tree. In this type of tree we use K to refer to the maximum number of children that each Node is able to have.

### Breadth First Traversal
Traversing a K-ary tree requires a similar approach to the breadth first traversal. We are still pushing nodes into a queue, but we are now moving down a list of children of length k, instead of checking for the presence of a left and a right child.


### Refrences
- https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html
- https://en.wikipedia.org/wiki/Tree_(data_structure)

## Read Trees link:
https://boodah96.github.io/reading-notes/text14