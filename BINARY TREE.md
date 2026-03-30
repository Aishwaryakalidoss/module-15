# Experiment 9(a): Binary Tree (Float Values)

## Aim
To write a Python program to build a binary tree with a root, left, and right node using float values.

---

## Algorithm

1. Start the program.
2. Import the `Node` class from the `binarytree` module.
3. Create a root node using the `Node` class and input a floating-point value for the root.
4. Create left and right child nodes for the root using floating-point values.
5. Convert the binary tree to a list.
6. Print the list of nodes.
7. End the program.

---

## Program

```python
from binarytree import Node

# Input float values for root and child nodes
from binarytree import build,Node

def bst(x):
    if len(x)==0:
        return None
    
    mid = len(x)//2
    root=Node(x[mid])
    root.left=bst(x[:mid])
    root.right=bst(x[mid+1:])
    return root 


l=[1,2,3,5,4,6]

print("BST before insertion:")
xbst=bst(sorted(l))
for i in xbst.values:
    print(i,"-->",end="")
    
print()
print("BST after insertion:")
l.append(int(input()))
xbst=bst(sorted(l))
for i in xbst.values:
    print(i,"-->",end="")

# Print the binary tree as a list

```

## OUTPUT
<img width="1185" height="270" alt="image" src="https://github.com/user-attachments/assets/1aec4dc7-8209-4d62-9645-82ee4f5fe93b" />


## RESULT
Therefore, the output is the example to write a Python program to build a binary tree with a root, left, and right node using floating-point values.
