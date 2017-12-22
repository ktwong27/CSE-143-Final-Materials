#Collections Mystery 005

```
public Map<String, String> mystery(Map<String, Integer> map1,
                                    Map<Integer, String> map2) {
    Map<String, String> result = new TreeMap<String, String>();
    for (String s1 : map1.keySet()) {
        if (map2.containsKey(map1.get(s1))) {
            result.put(s1, map2.get(map1.get(s1)));
        }
    }
    return result;
}
```

For each of the following, fill in the output printed when mystery is called on the given Collection.

| Input Collection        | Map Returned        |
| ------------- |:---------:|
| map1: {bar=1, baz=2, foo=3, mumble=4} <br> map2: {1=earth, 2=wind, 3=air, 4=fire}      | _______________________________ |
| map1: {five=105, four=104, one=101, six=106, three=103, two=102} <br> map2: {99=uno, 101=dos, 103=tres, 105=quatro}      | _______________________________      |
| map1: {a=42, b=9, c=7, d=15, e=11, f=24, g=7} <br> map2: {1=four, 3=score, 5=and, 7=seven, 9=years, 11=ago} | _______________________________      |