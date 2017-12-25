# oddDepthSum() Solution


```
public static int oddDepthSum(){
    return oddDepthSum(overallRoot, 1);
}

private static int oddDepthSum(IntTreeNode root, int cur){
    int count = 0;
    if (root != null) {
        if (cur % 2 ==1) {
            count += root.data;
        }
        count += oddDepthSum(root.left, cur + 1);
        count += oddDepthSum(root.right, cur + 1);
    }
    return count;
}
```