# Student Grade Monitoring System

Simple command-line Student Grade Monitoring System implemented in C++ using an AVL tree.

## Overview
- Maintains student records (student_ID, name, course, grade, GPA) in an AVL tree for balanced O(log n) insert/search/update/delete.
- Can save and load records to/from a CSV file.
- Menu-driven CLI for adding, updating, searching, deleting, displaying, saving, and loading records.

## Files
- `main.cpp` — CLI and input validation.
- `AVLTree.h` / `AVLTree.cpp` — AVL tree implementation and file I/O (save/load CSV).
- `AVLNode.h` / `AVLNode.cpp` — Node implementation for the AVL tree.
- `studentrecord1.csv` — example CSV data (if present).

## Build
### Prerequisites

- C++ compiler with C++11 support (g++, clang++, etc.)
- Make (optional, for using Makefile)

### Compilation Options


```powershell
cd c:\hmm\Team_PS5\PS5Unfucked
g++ -o program.exe main.cpp AVLTree.cpp AVLNode.cpp -std=c++17
```


Follow the menu to add, update, search, delete, display, save, or load student records.

## CSV format
Each saved line is a CSV record with the fields in order:
```
student_ID,name,course,grade,GPA
```
Example:
```
12345,Jane Doe,Math 101,92.5,4.00
```
When saving/loading, provide the filename including extension (for example `data.csv`).

## Notes
- File I/O is handled by the `AVLTree` methods `saveToFile` and `loadFromFile`.
- The program expects filenames with an extension (like `.csv`) when saving/loading.

## Sources (pseudocode and algorithms)
The algorithm references used in the project are from GeeksforGeeks as listed in the project document:

- "Insertion in an AVL Tree", GeeksforGeeks — https://www.geeksforgeeks.org/dsa/insertion-in-an-avl-tree/
- "Deletion in an AVL Tree", GeeksforGeeks — https://www.geeksforgeeks.org/dsa/deletion-in-an-avl-tree/
- "Search in an AVL Tree", GeeksforGeeks — https://www.geeksforgeeks.org/dsa/avl-trees-containing-a-parent-node-pointer/
- "Inorder Traversal of Binary Tree", GeeksforGeeks — https://www.geeksforgeeks.org/dsa/inorder-traversal-of-binary-tree/


## Authors
Team PS5

## License
This project is created for educational purposes as part of CSC 307 coursework.

## Acknowledgement
- Course Instructor: Prof. Chad McDaniel
- GeeksforGeeks for AVL Tree algorithm references
- Team PS5 members for collaborative design and implementation

---

**End of Documentation**
