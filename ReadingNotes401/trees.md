# [Trees](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)

**node** - an item or piece of data that makes the data structure

**Root** - the *first* node at the top of a tree

**Left/Right Child** - node to the left or right of it's parent node

**Edge** - The link between a parent and child node

**Leaf** - A node that does not have any children

**Height** - The *number* of edges from the root node to the lowest node


## Binary Trees

While **trees** can have any number of children per node, **binary trees** can only have two- a right and a left child. Nodes can be added to a tree wherever there is space, there is no specific sorting order.

### Adding a Node

It doesn't matter *how* a new node gets added to a binary tree. But for example you can fill *child* spots from the top down.

1. find the first node **without two children**
2. add new node as a child
3. add children going from *left to right*

### Big O

**For time:** 
- inserting a node = O(n)
- searching for node = O(n)

A binary tree isn't really organized, assuming a tree has `n` node, you might have to look at `n` number of items in order to find that **one**.

**For space using breadth-first:**

- inserting a node = O(w)

`w` being the *largest* **width** of the tree.

**Perfect Binary Tree?**

When every node that **isn't** a leaf has **two** children, therefor- the *maximum width* for a perfect tree is `2^(h-1)`. `h`=height, height being calculated as `log n`, where `n` is the number of nodes.

## Binary Search Tree (BST)

A BST **does** have some structure. The nodes are organized where values that are **less than** the root/parent become the **left child**, while those values which are greater are assigned as the **right child**

### Searching a BST

Compare the node you are looking for against the root/root of a sub-tree to determine if the value is *greater than* or *less than*. If less, traverse left, if greater, traverse right.

#### Big O?

**For time:**

- inserting/searching a node = O(h)

in a perfect tree. the h = log(n)

**For space:**

- searching a node = O(1)

because we are not allocating *additional* space


## Traversing Trees

### Depth First (finding the height of the tree first)

Three methods for depth first traversal:

#### 1. PRE-ORDER BREAKDOWN:

`root>>left>>right` ex: `A,B,D,E,C,F`

The root must be looked at first and output it's value will be added to the call stack each time preOrder is called.

1. output value of root to console
2. if left root *has* a value, send it to preOrder method
3. B becomes *new* root and has it's value added to call stack
4. Once `root.left/root.right` return **null**, you know you are at the **leaf** and the execution will end.
5. The leaf is removed from the call stack, and the root is reassigned to the previous parent that **does** have a left and right-and it will look **right** instead.
6. if the right is *also* a leaf, it will be removed from the stack as well and the the previous parent node will once again be reassigned as the **root** - **BUT**, since the left *and* right of the parent have already been checked, the current root will also be removed from the call stack and *its* parent will once again become the root node that will then go **right** instead of left this time.

**algorithm for pre-order**

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

**OTHER ALGORITHMS FOR DEPTH FIRST, DIFFERENCE IS *WHEN YOU ARE LOOKING AT ROOT NODE DURING TRAVERSAL***

**algorithm for in-order**

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

**algorithm for post-order**

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

### Breadth First (going through each level node by node)

#### 1. BREADTH-FIRST BREAKDOWN:

`root>>left & right` ex: `A,B,C,D,E,F`

Different from depth-first in that it uses a queue instead of a (call) stack in order to traverse the width&breadth of tree.

1. **Root** is added to queue(therefor,at the front)
2. *Then* dequeue the node just added to queue and use it in code to `enqueue` it's **left** (first) and **right** (second) children.
3. AT THIS POINT, THE LEFT NODE SHOULD BE THE FRONT OF THE QUEUE AND THE RIGHT NODE SHOULD BE SECOND IN LINE.
4. **Then** do the same thing in step two, dequeue the **front** node and enqueue *its* left and right children.
5. Once a node is reached that **does not** have children, just dequeue it.

**algorithm for breadth-first**

  ```
ALGORITHM breadthFirst(root)
// INPUT  <-- root node
// OUTPUT <-- front node of queue to console

  Queue breadth <-- new Queue()
  breadth.enqueue(root)

  while breadth.peek()
    node front = breadth.dequeue()
    OUTPUT <-- front.value

    if front.left is not NULL
      breadth.enqueue(front.left)

    if front.right is not NULL
      breadth.enqueue(front.right)
```


