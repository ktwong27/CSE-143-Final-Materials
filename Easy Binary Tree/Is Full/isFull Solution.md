# isFull() Solution

One possible solution is as follows:
```
 public static boolean isFull() {
     return isFull(overallRoot);
 }
 private static boolean isFull(IntTreeNode root) {
     if (root != null) {
         if ((root.left == null && root.right != null) || (root.left != null && root.right == null)) {
             return false;
         } else {
             return isFull(root.left) && isFull(root.right);
         }
     }
     return true;
 }
```