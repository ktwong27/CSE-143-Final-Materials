# nodesAtLevels() Solution


```
public static int nodesAtLevels(int start, int stop) {
    return nodesAtLevels(start, stop, 0, overallRoot);
}

private static int nodesAtLevels(int start, int stop, int cur, IntTreeNode root) {
    int count = 0;
    if (root != null) {
        if (cur < start) {
            count += nodesAtLevels(start, stop, cur + 1, root.left);
            count += nodesAtLevels(start, stop, cur + 1, root.right);
        } else if (start <= cur && cur <= stop) {
            count++;
            count += nodesAtLevels(start, stop, cur + 1, root.left);
            count += nodesAtLevels(start, stop, cur + 1, root.right);
        }
    }
    return count;
}
```