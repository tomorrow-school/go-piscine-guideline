
# Quest 12

Quest 12 is focused on binary search trees (BST), a fundamental data structure in computer science. These tasks teach you how to construct, traverse, modify, and query binary trees in Go, strengthening your understanding of pointers, recursion, and tree algorithms. Here’s an overview of the key concepts and recommended learning resources:

***

### Key Concepts

- **Binary Search Tree Structure**
    - Each node stores data and links to its left and right children, obeying the BST property: left child < parent < right child.[^1][^2][^3]
    - Parent pointers enable upward navigation for some operations.
- **Insertion, Deletion, and Transplant**
    - Insertions keep the tree sorted for fast search.
    - Deleting nodes and transplanting subtrees require careful pointer management; these operations must preserve BST properties.[^4][^5][^6][^7]
- **Tree Traversals**
    - In-order (Left, Root, Right): retrieves sorted data from the BST.[^8][^9][^10]
    - Pre-order (Root, Left, Right) and by-level (breadth-first): process nodes in specific orders for display or other algorithms.
- **Searching \& Min/Max**
    - Efficiently find nodes or minimum/maximum values by traversing down the left/right subtree as appropriate.[^11][^12]
- **Tree Height \& Levels**
    - Understanding tree depth (number of levels) is important for performance analysis and further tree algorithms.[^13]
- **Generic Data \& Function Application**
    - Each node contains a string (or, in general, comparable data), and tasks involve applying functions to tree nodes as you traverse.

***

### Recommended Learning Resources

- **Go Data Structures: Binary Search Tree (Flavio Copes)**
Introductory and practical guide for BSTs in Go, including code samples for insertion, search, and traversals.[^1]
- **Implementing a Binary Search Tree in Go (Substack, Nuwan)**
Walks through generic implementations and different BST operations with Go code.[^2]
- **GoLang Tutorial - Binary Search Tree (Bogotobogo)**
Provides foundational explanations and code for building and manipulating BSTs in Go.[^3]
- **Data Structures in Golang - Binary Search Tree (YouTube)**
Video tutorial explaining BST concepts and code in detail.[^14]
- **Binary Tree Traversals in Go (CodeSignal Learn)**
Covers in-order, pre-order, and post-order traversals in Go.[^10]
- **Golang program to perform inorder/preorder tree traversal (TutorialsPoint)**
Explains algorithms and Go code for in-order and pre-order traversals.[^15][^8]
- **Binary Search Trees 8 - Deletions and Transplanting Nodes (YouTube)**
Visual explanation of transplant and node deletion operations in BSTs.[^6]
- **Deletion in Binary Search Tree (GeeksforGeeks)**
Deep dive into the algorithm for deleting various types of nodes from BSTs.[^7]

***

### Additional Notes

- Working with binary search trees builds your skills in recursive thinking, pointer manipulation, and designing efficient search algorithms.
- Practical experience with BST operations is foundational for interviews, algorithmic challenges, and real-world tasks like data indexing and retrieval.
- These tasks expose common patterns in Go for data structure implementation and manipulation, especially recursive function design.

Utilize these resources for detailed explanations, example code, and hands-on exercises to solidify your knowledge and problem-solving skills in BSTs with Go.
<span style="display:none">[^16][^17][^18][^19][^20]</span>

<div style="text-align: center">⁂</div>

[^1]: https://flaviocopes.com/golang-data-structure-binary-search-tree/

[^2]: https://datastructures.substack.com/p/implementing-a-binary-search-tree-in-golang

[^3]: https://www.bogotobogo.com/GoLang/GoLang_Binary_Search_Tree.php

[^4]: https://www.cs.dartmouth.edu/~thc/cs10/lectures/0502/0502.html

[^5]: https://stackoverflow.com/questions/66536347/delete-function-binary-search-tree-bst-with-parent-passing-the-tree-pointer-as-a

[^6]: https://www.youtube.com/watch?v=NNvM3ZSr9dY

[^7]: https://www.geeksforgeeks.org/dsa/deletion-in-binary-search-tree/

[^8]: https://www.tutorialspoint.com/golang-program-to-perform-inorder-tree-traversal

[^9]: https://www.youtube.com/watch?v=0AucCCwmpnw

[^10]: https://codesignal.com/learn/courses/getting-deep-into-complex-algorithms-for-interviews-with-go/lessons/binary-tree-traversals-in-go

[^11]: https://blog.devgenius.io/bst-implementation-in-golang-fb92309fe96a

[^12]: https://kaperys.io/2021-08-03-implementing-a-binary-search-tree-in-go

[^13]: https://epigra.com/en/blog/understanding-binary-search-trees-with-basic-implementation-in-golang

[^14]: https://www.youtube.com/watch?v=Id099WXOKNM

[^15]: https://www.tutorialspoint.com/golang-program-to-perform-the-preorder-tree-traversal

[^16]: https://www.tutorialspoint.com/golang-program-to-delete-a-node-from-a-red-black-tree

[^17]: https://www.tutorialspoint.com/golang-program-to-check-if-a-binary-tree-is-a-binary-search-tree

[^18]: https://habr.com/en/articles/545980/

[^19]: https://pkg.go.dev/github.com/mikenye/gotrees/bst

[^20]: https://dhdersch.github.io/golang/2022/07/16/decouple-depth-first-traversal-algorithm-from-business-logic.html

