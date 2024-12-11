## Problem Description  

You are given the root of a binary tree. Your task is to determine whether the binary tree is **symmetric** around its center, i.e., if it is a mirror of itself.  

---

### Solution Approach  

The solution uses a recursive function to check if the left and right subtrees of the root are mirrors of each other.  

**Steps**:  
1. **Base Case**:  
   - If the tree is empty (`root == null`), it is symmetric.  
2. **Recursive Check**:  
   - Use a helper function `isMirror` to verify:  
     - The values of the current nodes in the left and right subtrees are equal.  
     - The left child of the left subtree is a mirror of the right child of the right subtree.  
     - The right child of the left subtree is a mirror of the left child of the right subtree.  
3. Return `true` if all conditions are satisfied.  

---

### Time and Space Complexity  

- **Time Complexity**: O(n), where `n` is the number of nodes in the binary tree. Each node is visited once.  
- **Space Complexity**: O(h), where `h` is the height of the tree, for the recursive call stack.  

---

For a detailed explanation of the approach, visit the [description here](https://leetcode.com/problems/symmetric-tree/description/).
