#Collections Mystery 015

```
public static void mystery(List<Integer> list) {
    Map<Integer, Integer> result = new TreeMap<Integer, Integer>();
    
    while (!list.isEmpty()) {
        Iterator<Integer> it = list.iterator();
        
        while (it.hasNext()) {
            int i = it.next();
            if (i % 2 == 0) {
                if (!result.containsKey(i)) {
                    result.put(i, 0);
                }
                result.put(i, result.get(i) + 1);
            }
            it.remove();
        }
    }
    
    System.out.println(result);
}
```

For each of the following, fill in the output printed when mystery is called on the given Collection.

| Input Collection        | Output Map         |
| ------------- |:---------:|
| [1, 1]       | _______________________________ |
| [200, 200, 300, 400]      | _______________________________      |
| [1, 2, 1, 2] | _______________________________      |
| [9, 8, 7, 6, 5, 4]Collections Mystery 015 | _______________________________      |