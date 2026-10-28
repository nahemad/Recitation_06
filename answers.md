# CMPS 2200 Recitation 06
## Answers

**Name:** Nahema Dumonteil 
**Name:**_________________________


Place all written answers from `recitation-06.md` here for easier grading.



- **1)** Before we implement a heap, let's consider if we just maintain
 an unordered list/sequence. 

  - **1a) (1 pt)** What is the work/span of *deleteMin*?
  Do delete a min we first need to find a min. Finding a min in an unsorte dlist takes work, O(n) and then deleting an element form a list also takes work O(n), so the total work is O(n).
  Span would also be O(n) because if we use a loop to find the min, it would be a sequential prcoess. 

  - **1b) (1 pt)** What is the work/span ofand *insert(x)*?
  To insert an element, if it is at the end of the list then it takes constant time O(1). To insert in the middle or other implementatons can be linear time. so the work would be O(1) or O(n) 
  Span would also be O(1) because we are still just appending an element at the end of the list (its an independent step)

- **2a) (1 pt)** For a heap with $n$ elements, what does this imply about the depth of the associated almost-complete binary tree? 
almost-complete means the last level is not completly filled form left to right. This means the trees debth is bounded by log(n) because it can't go to the next level until it is filled from left to right. 

- **2b) (1 pt)** By maintaining the heap property, where is the minimum element of
  the heap? Can we say anything about the maximum element?
The minimum will be at the very first node at the top. The only thing we can say about the maximum is where it could be located. We know it has to be a node with no children. 
- **4a) (1 pt)** What is the work/span of *reheapUp*($x$)?
Work and Span are both O(logn) because the woest case is that the inserted node is the minimum in which case it has to jump all the way up passing throught he whole lengt/depth of the binary tree. This process is sequential so the Span stays the same
- **4b) (1 pt)** What is the work/span of *reheapDown*($x$)? 
Work and Span are both O(logn) because the woest case is that the inserted node is one of the bigger ones, in which case it has to jump all the way down passing through the whole lengt/depth of the binary tree. This process is sequential so the Span stays the same
- **6) (1 pt)** What is the work and span of `heapsort`?
Building the heap requres to insert n elements where each insertion take sup to O(logn) so basically n times log n. Same for deleting each element, its n elements and each tage logn work. Adding this is O(nlogn) +O(nlogn) = O(2nlogn) which is simoly O(nlogn)

The span is also going to be O(nlogn) because this is a sequential process. Each insertion and deletion happen one after the other.  