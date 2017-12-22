<div class="viewer">

### purebredOdds

<div>

Write a method purebredOdds that returns the number of purebred odd values in a binary tree of integers. A purebred odd is an odd number all of whose ancestors in the tree are also odd numbers. For example, suppose that a variable t refers to the following tree:

                                  +----+
                                  | 15 |
                                  +----+
                                /        \
                              /            \
                       +----+                +----+
                       | 27 |                | 34 |
                       +----+                +----+
                      /      \                     \
                     /        \                     \
                 +----+      +----+                +----+
                 | 29 |      | 75 |                | 83 |
                 +----+      +----+                +----+
                            /      \              /      \
                           /        \            /        \
                       +----+      +----+    +----+      +----+
                       | 18 |      | 33 |    | 46 |      | 51 |
                       +----+      +----+    +----+      +----+

Then the call t.purebredOdds() should return 5 because this tree has a total of 5 purebred odd values: 15, 27, 29, 75, and 33\. The values 83 and 51 are odd numbers, but not purebred odd numbers because they have an even number as an ancestor in the tree (the value 34). Notice that if the overall root is an even number, then the tree will have no purebred odd numbers at all because every other node has the overall root as an ancestor.

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