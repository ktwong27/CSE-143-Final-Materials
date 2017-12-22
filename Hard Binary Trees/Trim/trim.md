<div class="viewer">

### trim

<div>

Write a method trim that could be added to the IntTree class from lecture and section. The method accepts minimum and maximum integers as parameters and removes from the tree any elements that are not within that range, inclusive. For this method you should assume that your tree is a binary search tree (BST) and that its elements are in valid BST order. Your method should maintain the BST ordering property of the tree.

For example, suppose a variable of type IntTree called tree stores the following elements:

                             +----+
                             | 50 |
                       _____ +----+ _____
                      /                  \
                  +----+                   +----+
                  | 38 |                   | 90 |
            _____ +----+               ___ +----+
           /           \              /
        +----+         +----+   +----+
        | 14 |         | 42 |   | 54 |
        +----+         +----+   +----+
       /      \                      \
    +----+   +----+                  +----+
    |  8 |   | 20 |                  | 72 |
    +----+   +----+                  +----+
                  \                  /    \
                +----+           +----+  +----+
                | 26 |           | 61 |  | 83 |
                +----+           +----+  +----+

The table below shows what the state of the tree would be if various trim calls were made. The calls shown are separate; it's not a chain of calls in a row. You may assume that the minimum is less than or equal to the maximum.

           tree.trim(25, 72);           tree.trim(54, 80);          
                +----+                        +----+                       
                | 50 |                        | 54 |                      
              _ +----+                        +----+                  
             /        \                            \                     
        +----+        +----+                       +----+          
        | 38 |        | 54 |                       | 72 |          
        +----+        +----+                       +----+          
        /    \            \                        /                                 
    +----+  +----+       +----+                +----+                         
    | 26 |  | 42 |       | 72 |                | 61 |                          
    +----+  +----+       +----+                +----+                          
                          /   
                       +----+
                       | 61 |
                       +----+

           tree.trim(18, 42);            tree.trim(-3, 6);
                 +----+  
                 | 38 |  
                _+----+   
              /         \    
           +----+      +----+     
           | 20 |      | 42 |
           +----+      +----+
              \
              +----+  
              | 26 | 
              +----+ 

Hint: The BST ordering property is important for solving this problem. If a node's data value is too large or too small to fit within the range, this may also tell you something about whether that node's left or right subtree elements can be within the range. Taking advantage of such information makes it more feasible to remove the correct nodes.

You may define private helper methods to solve this problem, but otherwise you may not call any other methods of the class nor create any data structures such as arrays, lists, etc.

Recall the IntTree and IntTreeNode classes as shown in lecture and section:

    public class IntTreeNode {
        public int data;          // data stored in this node
        public IntTreeNode left;  // reference to left subtree
        public IntTreeNode right; // reference to right subtree

        public IntTreeNode(int data) { ... }
        public IntTreeNode(int data, IntTreeNode left, IntTreeNode right) {...}
    }

    public class IntTree {
        private IntTreeNode overallRoot;

        methods
    }

</div>

</div>