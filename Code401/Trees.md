# Trees

**Trees** are a fundamental data structure in computer science that have various applications. They are used to represent hierarchical relationships between objects or to organize data in a hierarchical manner. In a tree data structure, nodes are connected by edges, and each node (except the root) has a parent node and zero or more child nodes.

**key terms associated with trees:**

**Node** - A Tree node is a component which may contain its own values, and references to other nodes

**Root** - The root is the node at the beginning of the tree

**K** - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.

**Left** - A reference to one child node, in a binary tree

**Right** - A reference to the other child node, in a binary tree

**Edge** - The edge in a tree is the link between a parent and child node

**Leaf** - A leaf is a node that does not have any children

**Height** - The height of a tree is the number of edges from the root to the furthest leaf

**Binary Search Tree (BST):** A binary search tree is a binary tree in which the left child of a node contains a value less than the node's value, and the right child contains a value greater than the node's value. This property allows for efficient searching, insertion, and deletion operations.

**Balanced Tree:** A balanced tree is a tree in which the heights of the left and right subtrees of any node differ by at most one. Examples of balanced trees include AVL trees and red-black trees, which provide efficient operations even with dynamic data.

**Traversals**
* Depth First:Depth first traversal is where we prioritize going through the depth (height) of the tree first

 * Pre-order: root >> left >> right
 * In-order: left >> root >> right
 * Post-order: left >> right >> root
 
pseudocode for this traversal method:
**Pre-order**
```
ALGORITHM preOrder(root)
// INPUT <-- root node
// OUTPUT <-- pre-order output of tree node's values

    OUTPUT <-- root.value

    if root.left is not Null
        preOrder(root.left)

    if root.right is not NULL
        preOrder(root.right)
```

**In-order**
```
ALGORITHM inOrder(root)
// INPUT <-- root node
// OUTPUT <-- in-order output of tree node's values

    if root.left is not NULL
        inOrder(root.left)

    OUTPUT <-- root.value

    if root.right is not NULL
        inOrder(root.right)
```

**Post-order**
```
ALGORITHM postOrder(root)
// INPUT <-- root node
// OUTPUT <-- post-order output of tree node's values

    if root.left is not NULL
        postOrder(root.left)

    if root.right is not NULL
        postOrder(root.right)

    OUTPUT <-- root.value
```

* Breadth First: Breadth first traversal iterates through the tree by going through each level of the tree node-by-node.

**Pseudocode**
```
ALGORITHM breadthFirst(root)
// INPUT  <-- root node
// OUTPUT <-- front node of queue to console

  Queue breadth <-- new Queue()
  breadth.enqueue(root)

  while ! breadth.is_empty()
    node front = breadth.dequeue()
    OUTPUT <-- front.value

    if front.left is not NULL
      breadth.enqueue(front.left)

    if front.right is not NULL
      breadth.enqueue(front.right)
```

**K-ary Trees**
If Nodes are able have more than 2 child nodes, we call the tree that contains them a K-ary Tree. In this type of tree we use K to refer to the maximum number of children that each Node is able to have.

**Pseudocode**

```
ALGORITHM breadthFirst(root)
// INPUT  <-- root node
// OUTPUT <-- front node of queue to console

  Queue breadth <-- new Queue()
  breadth.enqueue(root)

  while ! breadth.is_empty()
    node front = breadth.dequeue()
    OUTPUT <-- front.value

    for child in front.children
        breadth.enqueue(child)
```

![img](https://www.tutorialspoint.com/assets/questions/media/41120/k_ary_tree.jpg)

