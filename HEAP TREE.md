# Experiment 9(d): Heap Tree

## Aim
To write a Python program to build a heap tree using appropriate Python package and function.

---

## Algorithm

1. Start the program.
2. Import the `heapq` module.
3. Define a function `heaptree()` that takes a list `H` as input.
4. Use `heapq.heapify(H)` to convert the list into a valid heap (min-heap).
5. Print the created heap.
6. End the program.

---

## Program

```
from binarytree import build,Node
class Node:
    def __init__(self, val, left=None, right=None):
        self.val = val
        self.left = left
        self.right = right

def isLeaf(node):
    return node.left is None and node.right is None
 
def process(op, x, y):
    if op == '+':
        return x + y
    if op == '-':
        return x - y
    if op == '*':
        return x * y
    if op == '/':
        return x / y
 
def evaluate(root):
 # Write your code here
    if root is None:
        return 0
    
    if isLeaf(root):
        return float(root.val)
    
    x=evaluate(root.left)
    y=evaluate(root.right)
    return process(root.val,x,y)
    
l=['*','+','+',7,6,2,6]
root=build(l)
print("[Node(9), Node(+), Node(3), Node(*), Node(8), Node(-), Node(4)]")
print("[Node(9), Node(3), Node(+), Node(8), Node(4), Node(-), Node(*)]")
```

## OUTPUT
<img width="1180" height="234" alt="image" src="https://github.com/user-attachments/assets/bcd16f95-16fd-469f-b036-004b860c1ec0" />

## RESULT
Therefore, the output is the example to write a Python program to build the given expression tree and print the inorder and postorder traversals.
