# Queue
**Basic Operations on Queue:**  
- **push():** Adds an element to the rear of the queue.
- **pop():** Removes an element from the front of the queue.
- **front():** Returns the front element of the queue without removing it.
- **isEmpty():** Returns true if the queue is empty, otherwise false.
- **isFull():** Returns true if the queue is full, otherwise false.

## Types of Queues

### **Simple Queue**
**Characteristics:** Elements are inserted from the rear and removed from the front.  
**Applications:**
- Print queue management.
- Process scheduling in operating systems.

### **Double-Ended Queue (Deque)**
**Characteristics:** Elements can be inserted or removed from both ends.
**Applications:**
- Storing history in web browsers.
- Managing tasks with varying priorities.

### Priority Queue
**Characteristics:** Elements are inserted with a priority. Higher priority elements are dequeued before lower priority ones.
**Applications:**
- Dijkstra's shortest path algorithm.
- Event-driven simulation systems.

### Circular Queue
**Characteristics:** The last position connects back to the first position, forming a circle.
**Applications:**
- Buffer management in data streams.
- Traffic management in operating systems.
