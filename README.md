Here is your content formatted as a clear, **ready‑to‑submit** section with the **table already included**:

***

### Application of Trees (Binary Search Tree)

#### Scenario  
Consider a **student record management system** where each student is identified by a unique roll number.  
- New students are added → **Insert into BST**  
- Records need to be viewed in sorted order → **Inorder traversal**  
- A specific student record may need removal → **Delete operation**

A **Binary Search Tree (BST)** is used to efficiently manage these operations.

#### Justification  
Binary Search Tree is chosen because:  
- It maintains **sorted order automatically**  
- Allows **fast searching, insertion, and deletion**  
- Efficient for **dynamic datasets** (size not fixed)  
- Traversals provide structured outputs:
  - **Inorder** → Sorted data  
  - **Preorder / Postorder** → Tree structure understanding  

#### Algorithm

1. **Insertion**
   - Create a new node.  
   - If root is `NULL`, make the new node as root.  
   - Compare data:  
     - If smaller → go to left subtree.  
     - If larger → go to right subtree.  
   - Repeat until correct position is found.  
   - Insert the node.

2. **Inorder Traversal (LNR)**
   - Traverse left subtree.  
   - Visit root.  
   - Traverse right subtree.  

3. **Preorder Traversal (NLR)**
   - Visit root.  
   - Traverse left subtree.  
   - Traverse right subtree.  

4. **Postorder Traversal (LRN)**
   - Traverse left subtree.  
   - Traverse right subtree.  
   - Visit root.  

5. **Deletion**
   - Search for the node.  
   - **Case handling:**
     - **Leaf node** → delete directly.  
     - **One child** → replace node with its child.  
     - **Two children** → replace node with its **inorder successor**.

***

### ⏱ Time Complexity

| Operation     | Average Case | Worst Case |
|---------------|--------------|------------|
| Insertion     | \(O(\log n)\) | \(O(n)\)   |
| Deletion      | \(O(\log n)\) | \(O(n)\)   |
| Searching     | \(O(\log n)\) | \(O(n)\)   |
| Traversals    | \(O(n)\)      | \(O(n)\)   |
