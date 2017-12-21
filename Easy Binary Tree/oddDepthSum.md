<div class="viewer">

### oddDepthSum

<div>

Write a method called oddDepthSum that returns the sum of the values of a binary tree of integers that occur at nodes with odd depth. More specifically, the overall root is considered to have a depth of 1, so it has an odd depth. It's children have a depth of 2, so they have even depth. The overall root's grandchildren have a depth of 3, so they have odd depth. And so on. For example, if the variable t refers to the following tree:

                                 +---+
                                 | 5 |
                                 +---+
                               /       \
                             /           \
                       +---+               +---+
                       | 1 |               | 3 |
                       +---+               +---+
                      /     \                   \
                     /       \                   \
                  +---+     +---+               +---+
                  | 2 |     | 4 |               | 8 |
                  +---+     +---+               +---+
                           /     \              /    \
                          /       \            /      \
                      +---+     +---+      +---+     +---+
                      | 0 |     | 9 |      | 6 |     | 7 |
                      +---+     +---+      +---+     +---+

Then the nodes with odd depth are those storing 5, 2, 4, and 8\. So the call t.oddDepthSum() would return 19\. If the tree is empty, the method should return 0.

You are writing a public method for a binary tree class defined as follows:

    public class IntTreeNode {
        public int data;          // data stored in this node
        public IntTreeNode left;  // reference to left subtree
        public IntTreeNode right; // reference to right subtree

        <constructors>
    }

    public class IntTree {
        private IntTreeNode overallRoot;

        <methods>
    }

You are writing a method that will become part of the IntTree class. You may define private helper methods to solve this problem, but otherwise you may not call any other methods of the class.

</div>

</div>