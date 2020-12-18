# [Stacks and Queues](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html)

## What is a stack?

A stack is a data structure made up of Nodes. A node in a  stack points at the next node but not the previous one. Common stack terminology:

**Push** - *nodes or items in a stack are pushed*

**Pop** - *nodes or items are removed*

**Top** 

**Peek** - *View the value of top node in stack*

**isEmpty** - *return true if empty stack, else false*

- **FILO**=First item added in stack will be the last one out.

- **LIFO**=Last item added in stack will be first popped out.

**PUSH**- *always* and O(1) operation. Takes same amount of time no matter how many nodes are in the stack.

  1. Assign *next* of node to be added to point at top node
  2. Reassign newly added node as *top*
  
  Pseudo:

    ```
    ALOGORITHM push(value)
    // INPUT <-- value to add, wrapped in Node internally
    // OUTPUT <-- none
    node = new Node(value)
    node.next <-- Top
    top <-- Node
    ```

**POP** - 0(1).

  1. Check `isEmpty` first to avoid exception
  2. Remove top node from stack and assign as **temp variable*
  3. Reassign next of former first as *top*
  4. Remove former top and clear next property of the current temp var
  5. Return value of former node that was popped off.

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

**PEEK** - O(1)
  1. Check `isEmpty` first to avoid exception

  ```
  ALGORITHM peek()
  // INPUT <-- none
  // OUTPUT <-- value of top Node in stack
  // EXCEPTION if stack is empty
  return top.value
  ```

**IsEmpty** - O(1)

  ```
  ALGORITHM isEmpty()
  // INPUT <-- none
  // OUTPUT <-- boolean
  return top = NULL
  ```


## What is a Queue?

**Enqueue** - Nodes/items added to queue

**Dequeue** - Nodes/items removed from queue

**Front** - First in queue

**Rear** - Last in queue

**Peek** - View value of first in queue

**IsEmpty** - Returns true if queue is empty, else false

- **FIFO** - First in First Out

- **LILO** - Last in Last Out

**Enqueue** - O(1), does not matter how many other items are in queue, takes same amount of time to perform operation.

1. Reference *next* of last node to reference new node
2. Reassign newly added node as *rear*

  ```
  ALGORITHM enqueue(value)
  // INPUT <-- value to add to queue (will be wrapped in Node internally)
  // OUTPUT <-- none
  node = new Node(value)
  rear.next <-- node
  rear <-- node
  ```

  **Dequeue** - O(1), does not matter how many items are in queue when you are always removing front node.

  1.Check `isEmpty`
  2. Make temp variable pointing at front node
  3. Reassign *next* of front node to become new *front*
  4. Reassign next property of temp var node to null.
  5. return temp node

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


