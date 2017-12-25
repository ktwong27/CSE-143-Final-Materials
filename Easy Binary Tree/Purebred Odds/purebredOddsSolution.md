# purebredOdds() Solution


```
public static int purebredOdds(){
    return purebredOdds(overallRoot);
}

private static int purebredOdds(IntTreeNode root){
    int count = 0;
    if (root != null && root.data % 2 == 1) {
        count++;
        count += purebredOdds(root.left);
        count += purebredOdds(root.right);
    }
    return count;
}
```