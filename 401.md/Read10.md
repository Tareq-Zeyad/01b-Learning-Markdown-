# Stacks and Queues


# Stacks

### What is a Stack?

### -A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack but DOES NOT reference its previous.
<br>

### Common methods that a stack must have

### 1- Push - Nodes or items that are put into the stack are pushed
### 2- Pop - Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.
### 3- Top - This is the top of the stack.
### 4- Peek - When you peek you will view the value of the top Node in the stack. When you attempt to peek at an empty stack an exception will be raised.
### 5- IsEmpty - returns true when the stack is empty otherwise returns false.
<br>


### Stacks follow 2 Important concepts:

```
FILO
First In Last Out

This means that the first item added in the stack will be the last item popped out of the stack.

LIFO
Last In First Out

This means that the last item added to the stack will be the first item popped out of the stack
```
<br>

### Big O of Stack Methods:

#### Push O(1)

### -Pushing a Node onto a stack will always be an O(1) operation. This is because it takes the same amount of time no matter how many Nodes (n) you have in the stack.

### When adding a Node, you push it into the stack by assigning it as the new top, with its next property equal to the original top.

### -algorithm of Push method in Pseudo Code
```
algorithm push(value)
// INPUT <-- value to add, wrapped in Node internally
// OUTPUT <-- none
   node = new Node(value)
   node.next <-- Top
   top <-- Node
```
<br>

#### Pop O(1)

### -Popping a Node off a stack is the action of removing a Node from the top. When conducting a pop, the top Node will be re-assigned to the Node that lives below and the top Node is returned to the user.

### Typically, you would check isEmpty before conducting a pop. This will ensure that an exception is not raised. Alternately, you can wrap the call in a try/catch block.

### -algorithm of Pop method in Pseudo Code
```
ALGORITHM pop()
// INPUT <-- No input
// OUTPUT <-- value of top Node in stack
// EXCEPTION if stack is empty

   Node temp <-- top
   top <-- top.next
   temp.next <-- null
   return temp.value
```
<br>

#### Peek O(1)

### -Returning the top of the stack element, however, we should check if the stack is empty or not first.

### -algorithm in Pseudo Code
```
ALGORITHM peek()
// INPUT <-- none
// OUTPUT <-- value of top Node in stack
// EXCEPTION if stack is empty

   return top.value
```
<br>

#### IsEmpty O(1)

### -Check if the stack is empty or not


### -algorithm of isEmpty in Pseudo Code
```
ALGORITHM isEmpty()
// INPUT <-- none
// OUTPUT <-- boolean

return top = NULL
```
<br>


# Queue

### What is an Queue?

### -A queue is a collection of objects that supports fast first-in, first-out (FIFO) semantics for inserts and deletes. The insert and delete operations are sometimes called enqueue and dequeue. Unlike lists or arrays, queues typically don't allow for random access to the objects they contain.


### Common methods for Queues

### 1- Enqueue - Add a new node to the queue.
### 2- Dequeue - Remove a node from the queue
### 3- Front - Return first node.
### 4- Rear - Return last node
### 5- Peek - Return the value of the first node.
### 6- IsEmpty - returns true when the queue is empty otherwise returns false.
<br>

### Queues also follow FILO and LIFO concepts.


### Big O of Stack Methods with Pseudo Code:

#### Enqueue O(1):

```
ALGORITHM enqueue(value)
// INPUT <-- value to add to queue (will be wrapped in Node internally)
// OUTPUT <-- none
   node = new Node(value)
   rear.next <-- node
   rear <-- node
```
<br>


#### Dequeue O(1):

```
ALGORITHM dequeue()
// INPUT <-- none
// OUTPUT <-- value of the removed Node
// EXCEPTION if queue is empty

   Node temp <-- front
   front <-- front.next
   temp.next <-- null

   return temp.value
```
<br>


#### Peek O(1):

```
ALGORITHM peek()
// INPUT <-- none
// OUTPUT <-- value of the front Node in Queue
// EXCEPTION if Queue is empty

   return front.value
```
<br>


#### IsEmpty O(1):

```
ALGORITHM isEmpty()
// INPUT <-- none
// OUTPUT <-- boolean

return front = NULL
```



