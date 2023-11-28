# JavaScript Queuing System

## Overview

This project provides a simple implementation of a queuing system in JavaScript. The `Queue` class allows you to create a queue, enqueue and dequeue elements, check the front element, and perform other basic queue operations.

## Table of Contents

- [Getting Started](#getting-started)
- [Usage](#usage)
- [Methods](#methods)
- [Example](#example)
- [Use Cases](#use-cases)
- [Contributing](#contributing)
- [License](#license)

## Getting Started

To use the queuing system in your JavaScript project, you can include the `Queue` class from the provided `queue.js` file.

```javascript
// Example import in your JavaScript file
const Queue = require('./path/to/queue');

// Your code here
```

## Usage

1. **Creating a Queue:**
   ```javascript
   const queue = new Queue();
   ```

2. **Enqueuing Elements:**
   ```javascript
   queue.enqueue(1);
   queue.enqueue(2);
   queue.enqueue(3);
   ```

3. **Dequeueing Elements:**
   ```javascript
   const dequeuedElement = queue.dequeue();
   ```

4. **Checking Front Element:**
   ```javascript
   const frontElement = queue.front();
   ```

5. **Checking if Queue is Empty:**
   ```javascript
   const isEmpty = queue.isEmpty();
   ```

6. **Getting Queue Size:**
   ```javascript
   const queueSize = queue.size();
   ```

7. **Printing the Queue:**
   ```javascript
   queue.printQueue();
   ```

## Methods

- **`constructor()`**: Initializes an empty queue.
- **`enqueue(element)`**: Adds an element to the end of the queue.
- **`dequeue()`**: Removes and returns the element at the front of the queue.
- **`front()`**: Returns the front element without removing it.
- **`isEmpty()`**: Checks if the queue is empty.
- **`size()`**: Returns the size of the queue.
- **`printQueue()`**: Prints the elements of the queue.

## Example

```javascript
const Queue = require('./path/to/queue');

const queue = new Queue();

queue.enqueue(1);
queue.enqueue(2);
queue.enqueue(3);

console.log("Front Element:", queue.front()); // Output: 1

const dequeuedElement = queue.dequeue();
console.log("Dequeued Element:", dequeuedElement); // Output: 1

console.log("Is Queue Empty:", queue.isEmpty()); // Output: false
console.log("Queue Size:", queue.size()); // Output: 2

queue.printQueue(); // Output: 2 3
```

## Use Cases

A queuing system is useful in various scenarios, including:

- Task scheduling: Processing tasks in a specific order.
- Breadth-first search in graph algorithms.
- Print job management: Handling print jobs in the order they are submitted.

## Contributing

Feel free to contribute to the project by submitting pull requests or opening issues. Follow the project's coding style and guidelines.


