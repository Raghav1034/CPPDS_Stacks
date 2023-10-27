# CPPDS_Stacks
# Cpp-Stacks

# Stack Implementation in C++

This C++ program demonstrates a basic implementation of a stack data structure. A stack is a fundamental data structure that follows the Last-In, First-Out (LIFO) principle, and it's used in various applications in computer science. In this program, we'll create a simple stack and provide algorithms for common stack operations.

## Stack Overview

### What is a Stack?

A **stack** is a linear data structure that follows the LIFO (Last-In, First-Out) principle. This means that the last element added to the stack is the first one to be removed. Imagine a stack of plates: you add a new plate on top and remove the topmost plate when needed. This characteristic is crucial for solving many algorithmic problems and managing data efficiently.

### Key Operations

In this implementation, we provide the following key stack operations:

1. **Push**: Add an element to the top of the stack.
2. **Pop**: Remove and return the top element from the stack.
3. **Peek (or Top)**: Return the top element without removing it.
4. **isEmpty**: Check if the stack is empty.
5. **Size**: Return the number of elements in the stack.

### Implementation

The stack is implemented using a dynamically allocated array. Here's a brief overview of the stack implementation:

- **Stack Initialization**: The stack is initialized with a given capacity, and a dynamic array is allocated to store the elements.

- **Push Operation**: Elements are added to the top of the stack. If the stack is full, it cannot push more elements.

- **Pop Operation**: The top element is removed and returned. If the stack is empty, there's nothing to pop.

- **Peek Operation**: The top element is returned without removing it. If the stack is empty, there's nothing to peek.

- **isEmpty Operation**: Checks if the stack is empty by examining the top index.

- **Size Operation**: Returns the number of elements currently in the stack.

### Algorithm
Data:
  - data: An array to store elements
  - top: A variable to keep track of the top element
  - capacity: Maximum number of elements the stack can hold

Functions:
  - Constructor Stack(capacity): Initialize the stack with the given capacity.
  - Destructor ~Stack(): Release allocated memory.
  - push(element): Add an element to the top of the stack.
  - pop(): Remove and return the top element from the stack.
  - peek(): Return the top element without removing it.
  - isEmpty(): Check if the stack is empty.
  - size(): Return the number of elements in the stack.

Algorithm Steps:

1. Create a class `Stack` with the following private data members:
   - int* data: An array to store elements.
   - int top: A variable to keep track of the top element.
   - int capacity: Maximum number of elements the stack can hold.

2. Implement the constructor `Stack(capacity)`:
   - Allocate memory for the stack data array of size `capacity`.
   - Initialize `top` to -1, indicating an empty stack.

3. Implement the destructor `~Stack()`:
   - Deallocate the memory for the data array to prevent memory leaks.

4. Implement the `push(element)` method:
   - Check if the stack is full (top == capacity - 1). If it is, return an error (overflow).
   - Increment `top` by 1.
   - Add the `element` to `data[top]`.

5. Implement the `pop()` method:
   - Check if the stack is empty (top == -1). If it is, return an error (underflow).
   - Retrieve the element at the top of the stack (data[top]).
   - Decrement `top` by 1.

6. Implement the `peek()` method:
   - Check if the stack is empty (top == -1). If it is, return an error (stack is empty).
   - Return the element at the top of the stack (data[top]).

7. Implement the `isEmpty()` method:
   - Return true if `top` is -1, indicating an empty stack. Otherwise, return false.

8. Implement the `size()` method:
   - Return `top + 1` to indicate the number of elements in the stack.

9. Provide a sample main program to demonstrate how to create a stack object, perform push, pop, and peek operations, and check if the stack is empty or retrieve its size.

10. Finally, handle memory cleanup in the destructor to avoid memory leaks.

The above algorithm outlines the basic structure and operations for a stack data structure in C++. You can now implement these operations in C++ code based on this algorithm.


## Output

This repository includes C++ implementations of linked lists for each type. You can explore the code to see how linked lists are implemented and how they can be used in your applications.

![Screenshot 2023-10-23 144549](https://github.com/Arjun378/Cpp-Stacks/assets/74441883/5475e7f6-23e3-4178-ac8c-79572539184e)


![Screenshot 2023-10-23 144611](https://github.com/Arjun378/Cpp-Stacks/assets/74441883/c6313d52-0e2b-4f48-aafa-34612e37b5ec)
