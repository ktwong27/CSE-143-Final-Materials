<div class="viewer">

### makeFull

<div>

Write a method called **makeFull** that could be added to the IntTree class from lecture and section (see cheat sheet). The method should turn a binary tree of integers into a full binary tree. A full binary tree is one in which every node has either 0 or 2 children. Your method should produce a full binary tree by replacing each node that has one child with a new node that has the old node as a leaf where there used to be an empty tree. The new node should store a value that indicates the level of the tree (-1 for the first level of the tree, -2 for the second level of the tree, and so on).

The following table shows the results of a call of your method on a particular tree:

    IntTree tree = new IntTree();
    ...
    tree.makeFull();

           tree before call 
               +----+
               | 12 |
               +----+
              /
         +----+
         | 29 |
         +----+

           tree after call
               +----+
               | -1 |
               +----+
              /      \
         +----+      +----+
         | 29 |      | 12 |
         +----+      +----+

The node storing 12 that used to be at the top of the tree is now a leaf where there used to be an empty tree. In its place at the top of the tree is a new node that stores the value -1 to indicate that it was added at level 1 of the tree.

Your method should perform this operation at every level of the tree. For example:

                       tree before call
                           +----+
                           | 12 |
                           +----+
                        /          \
                +----+                +----+
                | 28 |                | 19 |
                +----+                +----+
               /                     /
          +----+                +----+
          | 94 |                | 32 |
          +----+                +----+
         /      \                     \
    +----+      +----+                +----+
    | 65 |      | 18 |                | 72 |
    +----+      +----+                +----+

                       tree after call
                            +----+
                            | 12 |
                            +----+
                         /          \
                +----+                  +----+
                | -2 |                  | -2 |
                +----+                  +----+
               /      \                /      \
          +----+      +----+      +----+      +----+
          | 94 |      | 28 |      | -3 |      | 19 |
          +----+      +----+      +----+      +----+
         /      \                /      \
    +----+      +----+      +----+      +----+
    | 65 |      | 18 |      | 32 |      | 72 |
    +----+      +----+      +----+      +----+

Notice that two nodes were added at level 2, and one at level 3. You may define private helper methods to solve this problem, but otherwise you may not assume that any particular methods are available. **You may NOT change the data field of existing nodes in the tree** (what we called "morphing" in assignments 7 and 8). You will, however, construct new nodes containing negative values to be inserted into the tree and you will change the links of the tree to restructure the tree as described. For full credit, your solution must be recursive and properly use the x = change(x) pattern.

</div>

</div>