# Experiment 9(e): Expression Tree Evaluation

## Aim
To write a Python program to build and evaluate the given expression tree.

---

## Algorithm

1. Start the program.
2. Create nodes for operators and operands.
3. Build the expression tree by connecting the nodes in the correct hierarchical structure.
4. Define a recursive function `evaluate(root)`:
   - If the node is a number (leaf), return it as a float.
   - Else, recursively evaluate the left and right subtrees.
   - Apply the operator at the current node to the results.
5. Return the final result from the root node.
6. End the program.

---

## Program

```
from binarytree import heap,build,Node
def heaptree(L):
  x=L
  t=build(x)
  for i in t.values:
    print(i,"-->",end='')
  print("\nHeight : ",t.height)
  print("Is min heap? : ",t.is_min_heap)
  print("Is complete tree? : ",t.is_complete)

```

## OUTPUT
<img width="1183" height="283" alt="image" src="https://github.com/user-attachments/assets/a98c9379-c078-4f6b-80bc-12ecb0472a5b" />


## RESULT
Therefore, the output is the example to write a Python program to build a heap tree using appropriate Python package and function.

