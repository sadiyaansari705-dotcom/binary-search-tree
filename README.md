Check if a Binary Tree is a Binary Search Tree (BST) in C

This project demonstrates how to check whether a given Binary Tree satisfies the properties of a Binary Search Tree (BST) using recursion and range validation.

🧾 Program Description

The program:

Defines a Node structure with:

data

left pointer

right pointer

Dynamically creates a binary tree using malloc().

Uses a recursive function isBST() to verify whether the tree satisfies BST rules.

Prints whether the tree is a BST or not.

🌳 Binary Search Tree (BST) Property

For a tree to be a BST:

All nodes in the left subtree must be smaller than the root.

All nodes in the right subtree must be greater than the root.

Both left and right subtrees must also be BSTs.

🧠 Approach Used

The program uses the Range (Min-Max) Method:

isBST(root, min, max)

Each node must satisfy:

min < node->data < max

Left subtree is checked within range (min, root->data)

Right subtree is checked within range (root->data, max)

This ensures the entire tree follows BST rules, not just immediate children.

🌲 Example Tree Used
            50
           /  \
         30    70
        /  \   /  \
      20   40 60   80

This tree satisfies BST properties.

📤 Sample Output
Tree is a BST
🧠 Concepts Used

Binary Trees

Binary Search Trees

Recursion

Range Validation Technique

Dynamic Memory Allocation (malloc)

Header File <limits.h> for INT_MIN and INT_MAX

🚀 How to Run
🔹 Compile the Program
gcc main.c -o output
🔹 Run the Program
./output

(For Windows)

output.exe
📂 Project Structure
📁 check-bst-c
 ├── main.c
 └── README.md
⚠️ Notes

Uses INT_MIN and INT_MAX for initial range.

Time Complexity: O(n)

Space Complexity: O(h) (recursive stack height)

🔧 Possible Improvements

Add inorder traversal check method.

Take user input to build the tree dynamically.

Add function to free allocated memory.

Create menu-driven tree operations.

👨‍💻 Author


B.Tech Student

If you want, I can also provide:

⭐ BST insertion and deletion program

⭐ Full BST implementation

⭐ Comparison between Binary Tree and BST

⭐ Short lab submission version
