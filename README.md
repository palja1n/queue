# Queue Implementation in C++

**Name:** Pal Jain  
**PRN:** 24070123067  
**Class:** ENTC A3  
**Title:** Queue Implementation using Array in C++

---

## Aim
To implement a Queue data structure in C++ using arrays and perform fundamental operations like **enqueue**, **dequeue**, and **display**.

---

## Objectives
- To understand the working principle of a Queue (FIFO: First In, First Out).  
- To implement basic Queue operations (insertion, deletion, traversal) using arrays.  
- To examine the cases of **overflow** and **underflow** in queues.  
- To identify the drawbacks of a linear queue and its real-world applications.  
- To strengthen understanding of **OOP concepts** through classes in C++.  

---

## Theory
A **Queue** is a linear data structure that follows the **FIFO principle**. The element inserted first will always be removed first. This is opposite to a **Stack**, which works on the LIFO rule.  

### Important Terms
- **Front** → Index of the element that will be deleted first.  
- **Rear** → Index where the new element will be added.  
- **Enqueue (Insertion)** → Adds an element to the rear end.  
- **Dequeue (Deletion)** → Removes an element from the front end.  
- **Display** → Prints all current elements in the queue.  

### Properties of a Queue
- **Sequential access**: Elements are processed in order of arrival.  
- **Restricted operations**: Insert only at rear, delete only at front.  
- **Overflow**: When the array is full and insertion is not possible.  
- **Underflow**: When the queue is empty and deletion cannot be done.  

### Types of Queues
- **Simple Queue (Linear Queue)** – insertion at rear, deletion at front.  
- **Circular Queue** – optimizes unused space of linear queue.  
- **Priority Queue** – deletion is based on priority, not order.  
- **Deque (Double Ended Queue)** – insertion and deletion from both ends.  

➡️ This project deals with a **Simple Queue** using arrays.

---

## Stack vs Queue

| Feature        | Stack (LIFO)        | Queue (FIFO)          |
|----------------|---------------------|-----------------------|
| Insertion      | At the top          | At the rear           |
| Deletion       | From the top        | From the front        |
| Order of Access| Last In → First Out | First In → First Out  |
| Use Cases      | Function calls, Undo| Scheduling, Buffering |

---

## Algorithm
1. Initialize `front = -1` and `rear = -1`.  
2. **Enqueue (value):**  
   - If `rear == SIZE - 1`, report **Overflow**.  
   - Else increment `rear` and place value in `arr[rear]`.  
   - If `front == -1`, set `front = 0`.  
3. **Dequeue():**  
   - If `front == -1 OR front > rear`, report **Underflow**.  
   - Else delete the element at `arr[front]` and increment `front`.  
4. **Display():**  
   - If queue is empty, print a message.  
   - Otherwise, print elements from `front` to `rear`.  
5. Continue operations as directed in `main()`.  
6. End program.  

---

## Program Overview
- Created a **Queue class** with private members: `arr`, `front`, and `rear`.  
- Implemented functions for `enqueue`, `dequeue`, and `display`.  
- Tested functionality inside `main()` with example operations.  
- Demonstrated FIFO execution and handled **overflow/underflow** properly.  

---

## Key Concepts Applied
- **Encapsulation:** Queue defined inside a class.  
- **Data Structures:** Queue implemented via arrays.  
- **Conditional checks:** Handling special cases of overflow/underflow.  
- **Loops:** For traversal in display function.  
- **Macros:** `#define SIZE 5` to fix queue size.  

---

## Conclusion
Through this experiment, the working of a **queue using arrays in C++** was successfully implemented and tested.  

We observed:  
- Practical working of the **FIFO principle**.  
- Situations where overflow and underflow occur.  
- Advantages and limitations of a linear queue.  
- Benefits of implementing queues with class-based encapsulation.  

### Applications
Queues are widely used in:  
- **CPU scheduling**  
- **Printer management**  
- **Network buffering**  
- **Task scheduling**  
