# Experiment 9(b): Binary Search Tree

## Aim
To write a Python program to build a Binary Search Tree (BST) using a built-in function.

---

## Algorithm

1. Start the program.
2. Import the `Node` class from the `binarytree` module.
3. Define a function `_build_bst_from_sorted_values()` to build a BST recursively from a sorted list.
4. Define a function `left_subtree()` to print the values in the left subtree of the BST.
5. Accept input from the user for the number of elements.
6. Read the elements into a list.
7. Sort the list.
8. Build the BST by calling `_build_bst_from_sorted_values()` with the sorted list.
9. Print the postorder traversal of the BST.
10. Print the left subtree values.
11. Check and print whether the built tree is a Binary Search Tree.
12. End the program.

---

## Program

```
from binarytree import Node
root=Node(1)
root.left=Node(2)
root.right=Node(3)
root.left.left=Node(5)
root.left.right=Node(6)
print("Binary tree: ")
for i in (root.values):
    print(i,"-->",end="")
print("\nLeft Subtree: ")
for i in (root[1].values):
    print(i,"-->",end="")
```

## OUTPUT
<img width="1182" height="260" alt="image" src="https://github.com/user-attachments/assets/f93f4f06-f396-4cb3-b69f-df144696a6b5" />


## RESULT
Therefore, the output is the example to write a Python program to build a binary search tree using a built-in function.
