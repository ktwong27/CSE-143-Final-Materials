<div class="viewer">

### isFull

<div>

Write a method isFull that returns whether or not binary tree is full (true if it is, false otherwise). A full binary tree is one in which every node has 0 or 2 children. The QuestionTree of assignment #7 and the HuffmanTree of assignment #8 are examples of full binary trees. Below are examples of each.

              full tree                        not a full tree
                +---+                               +---+
                | 2 |                               | 7 |
                +---+                               +---+
               /     \                             /     \
              /       \                           /       \
          +---+       +---+                   +---+       +---+
          | 3 |       | 1 |                   | 4 |       | 0 |
          +---+       +---+                   +---+       +---+
         /     \                             /     \           \
        /       \                           /       \           \
    +---+       +---+                   +---+       +---+      +---+
    | 8 |       | 7 |                   | 9 |       | 2 |      | 8 |
    +---+       +---+                   +---+       +---+      +---+

The right-hand tree is not full because the node with 0 in it has one child. By definition, the empty tree is considered full.

Assume that you are writing a public method for a binary tree class defined as follows:

    public class TreeNode {
        public int data;       // data stored in this node
        public TreeNode left;  // reference to left subtree
        public TreeNode right; // reference to right subtree

        <constructors>
    }

    public class Tree {
        private TreeNode root;  // reference to the overall root

        <methods>
    }

You are writing a method that will become part of the Tree class. You may define private helper methods to solve this problem, but otherwise you may not call any other methods of the class.

</div>

</div>