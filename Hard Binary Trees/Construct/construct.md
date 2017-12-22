<div class="viewer">

### construct

<div>

Write a method construct that takes a sorted array of integers as a parameter and that constructs a balanced binary search tree containing those integers. The tree that is constructed should have the property that for every node in the tree, either the left and right subtrees have the same number of nodes or the left subtree has one more node than the right subtree.

For example, if an array called list stores the values (1, 2, 3, 4, 5, 6, 7) and the following call is made for a variable t of type Tree:

    t.construct(list);

Then t should store the following tree after the call is made:

                                 +---+
                                 | 4 |
                                 +---+
                               /       \
                             /           \
                       +---+               +---+
                       | 2 |               | 6 |
                       +---+               +---+
                      /     \             /     \
                     /       \           /       \
                  +---+     +---+     +---+     +---+
                  | 1 |     | 3 |     | 5 |     | 7 |
                  +---+     +---+     +---+     +---+

If the array had instead stored (3, 8, 19, 27, 34, 42, 49, 53, 67, 74), then the following tree would have been constructed:

                                  +----+
                                  | 42 |
                                  +----+
                                /        \
                              /            \
                       +----+                +----+
                       | 19 |                | 67 |
                       +----+                +----+
                      /      \              /      \
                     /        \            /        \
                 +----+      +----+    +----+      +----+
                 |  8 |      | 34 |    | 53 |      | 74 |
                 +----+      +----+    +----+      +----+
                /           /         /
               /           /         /
           +----+      +----+    +----+
           |  3 |      | 27 |    | 49 |
           +----+      +----+    +----+

Notice that when it is not possible to have left and right subtrees of equal size, the extra value always ends up in the left subtree, as in the overall tree which has 5 nodes in the left subtree and 4 in the right.

Assume that you are writing a public method for a binary tree class defined as follows:

    public class TreeNode {
        public int data;       // data stored in this node
        public TreeNode left;  // reference to left subtree
        public TreeNode right; // reference to right subtree

        // post: constructs a leaf node with given data
        public TreeNode(int data) {
            this(data, null, null);
        }

        // post: constructs a TreeNode with the given data and links
        public TreeNode(int data, TreeNode left, TreeNode right) {
            this.data = data;
            this.left = left;
            this.right = right;
        }
    }

    public class Tree {
        private TreeNode root;  // reference to the overall root

        <methods>
    }

This problem involves constructing a new tree from an array of values. If there are "n" values in the array, then you should construct exactly "n" tree nodes. The new tree should replace any old tree. You are not allowed to use any other data structures (arrays, lists, Strings, etc) to solve this problem, you are not allowed to alter the array that you are passed and your solution must run in O(n) time. You can, however, assume that the values in the array appear in sorted (nondecreasing) order.

You are writing a method that will become part of the Tree class. You may define private helper methods to solve this problem, but otherwise you may not call any other methods of the class.

</div>

</div>