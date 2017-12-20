<div class="viewer">

### expand

<div>

Write a method called expand that expands the tree so that every node has either two null children or two non-null children. That is, no node will have a single child when your method finishes executing. If you encounter a node with a single child subtree, you should create a copy of the expanded non-null subtree and set the null child to this new subtree. For example, suppose a variable t stores a reference to the following tree:

                                 +---+
                                 | 3 |
                                 +---+
                               /       \
                             /           \
                       +---+               +---+
                       | 2 |               | 6 |
                       +---+               +---+
                      /                   /
                    /                   /
                 +---+               +---+
                 | 1 |               | 4 |
                 +---+               +---+
                                          \
                                           \
                                          +---+
                                          | 5 |
                                          +---+

There are three nodes in this tree that have a single child: the nodes storing 2, 6, and 4\. Each of these nodes will have it's null child replaced by an expanded copy of the subtree beginning at it's non-null child. So after the call:

    t.expand();

The tree should look like this:

                                 +---+
                                 | 3 |
                                 +---+
                             /           \
                         /                   \
                     +---+                   +---+
                     | 2 |                   | 6 |
                     +---+                   +---+
                   /       \               /       \
                 /           \           /           \
              +---+         +---+     +---+          +---+
              | 1 |         | 1 |     | 4 |          | 4 |
              +---+         +---+     +---+          +---+
                                      /   \          /   \
                                     /     \        /     \
                                  +---+   +---+  +---+   +---+
                                  | 5 |   | 5 |  | 5 |   | 5 |
                                  +---+   +---+  +---+   +---+

You are writing a public method for a binary tree class defined as follows:

    public class IntTreeNode {
        public int data;          // data stored in this node
        public IntTreeNode left;  // reference to left subtree
        public IntTreeNode right; // reference to right subtree

        // post: constructs an IntTreeNode with the given data and links
        public IntTreeNode(int data, IntTreeNode left, IntTreeNode right) {
            this.data = data;
            this.left = left;
            this.right = right;
        }
    }

    public class IntTree {
        private IntTreeNode overallRoot;

        <methods>
    }

You are writing a method that will become part of the IntTree class. You may define private helper methods to solve this problem, but otherwise you may not assume that any particular methods are available. You are NOT to change the data field of the existing nodes in the tree. You will, however, construct new nodes to be inserted into the tree and you will change the links of the tree to include these new nodes.

</div>

</div>