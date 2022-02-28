# Linked Lists Notes

### Big O: Analysis of Algorithm Efficiency
- Big O(oh) notation is used to describe the efficiency of an algorithm or function. This efficiency is evaluated based on 2 factors:
1. Running Time (also known as time efficiency / complexity)
  The amount of time a function needs to complete.
2. Memory Space (also known as space efficiency / complexity)
   The amount of memory resources a function uses to store data and instructions.
- We  use the letter **n** to refer to the Input Size value.

## Linked List
-A Linked List is a sequence of **Nodes** that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the **next Node** in the link.
### Singly Linked list
- A Singly linked list means that there is only one reference, and the reference points to the **Next node** in a linked list.
### Node
- Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.
### Next 
- Each node contains a property called **Next**. This property contains the reference to the next node.
### Head
- The Head is a reference of type Node to the first node in a linked list.
### Current
- The Current is a reference of type Node to the node that is currently being looked at.
- When traversing, you create a new Current variable at the Head to guarantee you are starting from the beginning of the linked list.

### Traversal 
- When traversing a linked list, you are not able to use a foreach or for loop. We depend on the Next value in each node to guide us where the next reference is pointing
- If we accidentally end up trying to traverse on a node that is null, a NullReferenceException gets thrown and our program will crash/end.


##### The biggest differentiator between arrays and linked lists is the way that they use memory in our machines
- When an array is created, it needs a certain amount of memory. If we had 7 letters that we needed to store in an array, we would need 7 bytes of memory to represent that array. But, we’d need all of that memory in one contiguous block. That is to say, our computer would need to locate 7 bytes of memory that was free, one byte next to the another, all together, in one place
- On the other hand, when a linked list is born, it doesn’t need 7 bytes of memory all in one place. One byte could live somewhere, while the next byte could be stored in another place in memory altogether! Linked lists don’t need to take up a single block of memory; instead, the memory that they use can be scattered throughout.
- An O(1) function takes constant time, which is to say that it doesn’t matter how many elements we have, or how huge our input is: it’ll always take the same amount of time and memory to run our algorithm
- An O(n) function is linear, which means that as our input grows (from ten numbers, to ten thousand, to ten million), the space and time that we need to run that algorithm grows linearly.
- For Linked List we only need to know O(1) and O(n)


## Reference and Citation:
[Big O](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/big_oh.html)
[Linked List](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)
[Linked List Medium blog Part 1](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d)
[Linked List Medium blog Part 2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)