Program 1
Aim

To implement a Queue using an array in C++ with basic operations such as enqueue (insertion), dequeue (deletion), and display.

Theory

A Queue is a linear data structure that follows the FIFO (First In, First Out) principle.
The element that is inserted first will be removed first.
It has two ends:
Front: where elements are deleted (dequeue)

Rear: where elements are inserted (enqueue).
Types of Queue
Simple Queue – Basic linear structure with enqueue and dequeue.
Circular Queue – Overcomes wasted space problem of simple queue.
Priority Queue – Elements are dequeued based on priority.

Double-Ended Quue (Deque) – Insertion and deletion at both ends.

In this program:
We implement a Simple Queue using an array of fixed size (SIZE = 5).
Enqueue inserts an element at the rear.
Dequeue removes an element from the front.
If rear == SIZE-1, it causes overflow.
If front > rear, the queue is considered empty (underflow).
Time Complexity:
Enqueue: O(1)
Dequeue: O(1)
Display: O(n

Space Complexity: O(SIZE)
Algorithm

- Enqueue (Insert)
- Check if rear == SIZE-1. If yes, print Overflow and stop.
- If front == -1, set front = 0 (first element case).
- Increment rear by 1.
- Insert the new element at arr[rear].
-  Dequeue (Delete)
- Check if front == -1 OR front > rear. If yes, print Underflow and stop.
- Print the element at arr[front].
- Increment front by 1.
- Display
- End
Check if front == -1 OR front > rear. If yes, print Queue is empty.

Otherwise, traverse from front to rear and print each element.
