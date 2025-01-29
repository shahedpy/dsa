## Tree
### Binary Search Tree (BST)

**Characteristics:**
- Left child nodes contain values less than the parent.
- Right child nodes contain values greater than the parent.

**Operations:**
- Insert: Add a new node while maintaining BST properties.
- Search: Find a node by value.
- Delete: Remove a node and restructure the tree if necessary.

**Applications:**
- Searching and sorting.
- Hierarchical data storage.
- Range queries.

### Heap
**Characteristics:**
- A complete binary tree.
- Two types: Max-Heap (root is the largest) and Min-Heap (root is the smallest).

**Applications:**
- Priority queues.
- Heap sort algorithm.

### Huffman Coding Tree
**Purpose:** Compression of data using variable-length encoding.
**Algorithm:**
- Create a priority queue of nodes sorted by frequency.
- Build a tree by merging the two least frequent nodes iteratively.
- Assign binary codes to characters based on tree traversal.

**Applications:**
- Data compression (e.g., ZIP files).
- Encoding for efficient transmission.
