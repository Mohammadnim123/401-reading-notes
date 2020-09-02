# Trees

**Common Terminology**
**Node -** A node is the individual item/data that makes up the data structure
**Root -** The root is the first/top Node in the tree
**Left Child -** The node that is positioned to the left of a root or node
**Right Child -** The node that is positioned to the right of a root or node
**Edge -** The edge in a tree is the link between a parent and child node
**Leaf -** A leaf is a node that does not contain any children
**Height -** The height of a tree is determined by the number of edges from the root to the bottommost node

![dd](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/BinaryTree1.PNG)

**Traversals**
An important aspect of trees is how to traverse them. Traversing a tree allows us to search for a node, print out the contents of a tree, and much more! There are two categories of traversals when it comes to trees:


* **Depth first** traversal is where we prioritize going through the depth (height) of the tree first. There are multiple ways to carry out depth first traversal, and each method changes the order in which we search/print the root.


* **Breadth first** traversal iterates through the tree by going through each level of the tree node-by-node.

## Binary Trees
In all of our examples, we’ve been using a Binary Tree. Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our left and right children).

>There is no specific sorting order for a binary tree. Nodes can be added into a binary tree wherever space allows.

**Adding a node**
Because there are no structural rules for where nodes are “supposed to go” in a binary tree, it really doesn’t matter where a new node gets placed.

One strategy for adding a new node to a binary tree is to fill all “child” spots from the top down. To do so, we would leverage the use of breadth first traversal. During the traversal, we find the first node that does not have 2 child nodes, and insert the new node as a child. We fill the child slots from left to right.

>In the event you would like to have a node placed in a specific location, you need to reference both the new node to create, and the parent node upon which the child is attached to.

**Binary Search Trees**
A Binary Search Tree (BST) is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.