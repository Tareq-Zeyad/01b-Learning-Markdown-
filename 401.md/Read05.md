## **Linked Lists**
### A Linked List is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link.
![linked-list](https://media.geeksforgeeks.org/wp-content/cdn-uploads/gq/2013/03/Linkedlist_insert_middle.png)

### **Terminology:**
- ### *Linked List* - A data structure that contains nodes that links/points to the next node in the list.
- ### *Singly* - Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.
- ### *Doubly* - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.
- ### *Node* - Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.
- ### *Next* - Each node contains a property called Next. This property contains the reference to the next node.
- ### *Head* - The Head is a reference of type Node to the first node in a linked list.
- ### *Current* - The Current is a reference of type Node to the node that is currently being looked at. When traversing, you create a new Current variable at the Head to guarantee you are starting from the beginning of the linked list.

![linkedList](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/images/LinkedList1.PNG)

### **Linked lists are often used because of their efficient insertion and deletion. They can be used to implement stacks, queues, and other abstract data types.**
<br>

### *How can we traverse a linked list ?*
### **We can traverse a linked list using any type of loops, however the best way to approach a traversal is through the use of a while() loop. This allows us to continually check that the Next node in the list is not null. If we accidentally end up trying to traverse on a node that is null, a NullReferenceException gets thrown and our program will crash/end.**