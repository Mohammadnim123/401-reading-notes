# Linked Lists

**What is a Linked List**
A Linked List is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link.

>There are two types of Linked List - **Singly** and **Doubly**. We will be implementing a Singly Linked List in this implementation.

![ff](https://www.alphacodingskills.com/imgfiles/linked-list.PNG)

**Terminology:**

* Linked List - A data structure that contains nodes that links/points to the next node in the list.

* Singly - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.

* Doubly - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.

* Node - Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.

* Next - Each node contains a property called Next. This property contains the reference to the next node.

* Head - The Head is a reference type of type Node to the first node in a linked list.

* Current - The Current reference is a reference type of type Node that is currently being looked at. This node is traditionally used when traversing through a full linked list. When traversing, you typically reset the current to the head to guarantee you are starting from the beginning of the linked list.

**Traversal**

>When traversing a linked list, you are not able to use a foreach or for loop. We depend on the Next value in each node to guide us where the next reference is pointing. The Next property is exceptionally important because it will lead us where the next node is and allow us to extract the data appropriately.

>The best way to approach a traversal is through the use of a while() loop. This allows us to continually check that the Next node in the list is not null. If we accidentally end up trying to traverse on a node that is null, a NullReferenceException gets thrown and our program will crash/end.

>When traversing through a linked list, the Current node is the most helpful. The Current will tell us where exactly in the linked list we are and will allow us to move/traverse forward until we hit the end.

**Big O**
The Big O of time for Includes would be O(n). This is because, at its worse case, the node we are looking for will be the very last node in the linked list. n represents the number of nodes in the linked list.

The Big O of space for Includes would be O(1). This is because there is no additional space being used than what is already given to us with the linked list input.

**Adding a Node**
Adding O(1)

>Order of operations is extremely important when it comes to working with a Linked List. What I mean by this is you must be careful that all references to each link/node is properly assigned.

>An example can be with adding a node to a linked list. If we want to add a node with an O(1) efficiency, we have to replace the current Head of the linked list with the new node, without losing the reference to the next node in the list.

Here are the required steps to add a new node with an O(1) efficiency.

* Set Current equal to Head. This will guarantee us that we are starting from the very beginning.

* We can then instantiate the new node that we are adding. The values passed in as arguments into the Add() method will define what the value of the Node will be.

* newNode.Next by default is set to null. We want to set newNode.Next property to the same location that the Head node is pointing towards. Because Head is just a reference type, we will be assigning it to the same allocation in memory as the node it is pointing too. In this case, it’s Node1.

* At this point in the program we now “technically” have newNode at the beginning of the linked list, but we are not done yet. We now have to re-assign where Head is pointing too. Since Node1 is no longer the first node in the list, we want to re-assign Head to point at newNode.

* While we are at it, let’s just re-assign current as well to make sure should any further operation start at the new true start of the linked list.

**The Linked List image above is in the following state:**

Current is pointing to node3.

* node3.Next property is equal to node4.

* Since this is the node we want to insert before, we can now set our node6.Next property also to node4. We do this at the time the node is found to prevent setting node6.Next to a node that may not exist.

* Uh-Oh, now both node3 and node6 are pointing to the same next node. node6 is not quite fully apart of the linked list.

* Next, we have to adjust node3.Next to point to the newly created node, node6. Since we still have Current pointing to node3 this will be a straightforward transaction. We just simply tell Current (because it is pointing to the same memory location as node3) to change it’s Next to point to the new node (node6).

