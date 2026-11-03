# Self-Balancing Binary Search Tree

## 1. Project Overview

This project implements and compares a Plain Binary Search Tree (BST) and an AVL Tree using Python. The objective is to understand how tree balancing affects insertion, searching, deletion, and tree height.

The project uses sequential, random, and nearly sorted datasets of different sizes to evaluate the performance of both trees. A Treap is also implemented as the self-learning component.

## 2. Objectives

- Implement basic operations in a Plain BST.
- Implement an AVL Tree with balancing rotations.
- Generate datasets with different input orders.
- Compare BST and AVL Tree performance.
- Measure execution time, tree height, search comparisons, and rotations.
- Visualize the tree-height comparison using a graph.
- Explore Treap as an additional tree data structure.

## 3. Technologies Used

- **Programming Language:** Python
- **Libraries:** Pandas, Matplotlib, Random, Time
- **Environment:** Jupyter Notebook or Google Colab
- **Data Format:** CSV

## 4. Data Structures Implemented

### Plain Binary Search Tree (BST)

The Plain BST arranges smaller keys on the left and larger keys on the right. It supports insertion, searching, deletion, inorder traversal, and height calculation.

### AVL Tree

An AVL Tree is a self-balancing BST. It maintains the balance factor of each node and uses rotations to keep the tree balanced.

The four rotation cases are:

- Left-Left (LL)
- Right-Right (RR)
- Left-Right (LR)
- Right-Left (RL)

### Treap — Self-Learning Component

A Treap combines BST ordering with heap priorities. It assigns random priorities to nodes and uses left and right rotations to maintain the heap property.

The implementation demonstrates insertion, searching, rotations, inorder traversal, and height calculation.

## 5. Dataset Generation

Three types of datasets are generated:

1. **Sequential:** Patient IDs arranged in ascending order.
2. **Random:** Patient IDs arranged in random order.
3. **Nearly Sorted:** Patient IDs arranged mostly in ascending order, with some positions swapped.

The dataset sizes are:

- 1,000 elements
- 5,000 elements
- 10,000 elements

## 6. Project Files

| File Name | Description |
|---|---|
| `patient_dataset.csv` | Contains the generated datasets, including dataset size, dataset type, and patient ID. |
| `BST_AVL_Comparison.csv` | Stores the experimental performance results for BST and AVL Tree. |
| `README.md` | Describes the project, implementation, and results. |
| Python notebook (`.ipynb`) | Contains the implementation, experiments, and graph plotting code. |

## 7. Performance Evaluation

The Plain BST and AVL Tree are compared using the following metrics:

- **Insertion Time:** Time required to insert elements into the tree.
- **Tree Height:** Number of edges on the longest path from the root to a leaf.
- **Search Comparisons:** Average number of key comparisons during searching.
- **Rotations:** Number of balancing rotations performed by the AVL Tree.

A graph is plotted to compare the height of the Plain BST and AVL Tree for the sequential dataset.

## 8. How to Run the Project

1. Open the notebook in Jupyter Notebook or Google Colab.
2. Run the import and class-definition cells.
3. Generate the datasets and save them as `patient_dataset.csv`.
4. Run the BST and AVL Tree experiments.
5. Save the comparison results as `BST_AVL_Comparison.csv`.
6. Run the graph-plotting cell to visualize the results.
7. Run the Treap implementation to test the self-learning component.

## 9. Expected Outcome

The project demonstrates how input order affects a Plain BST and how AVL balancing helps control tree height. Sequential input can produce a highly skewed Plain BST, while an AVL Tree maintains logarithmic height. The experiments provide a practical comparison of their performance.

The Treap implementation provides additional understanding of randomized priorities and rotations in tree data structures.

## 10. Conclusion

This project provides practical experience in implementing and analyzing tree data structures. Comparing a Plain BST with an AVL Tree demonstrates the importance of balancing for efficient operations. Implementing a Treap as a self-learning component extends the understanding of alternative tree
