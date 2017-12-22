#Collections Mystery 002

```
public static void mystery (Map<String, String> m) {
    Set<String> s = new TreeSet<String>();
    
    for (String key : m.keySet()) {
        if (!m.get(key).equals(key)) {
            s.add(m.get(key));
        } else {
            s.remove(m.get(key));
        }
    }
    System.out.println(s);
}

```

For each of the following, fill in the output printed when mystery is called on the given Collection.

| Input Collection        | Output         |
| ------------- |:---------:|
| {sheep=wool,
    house=brick,
    cast=plaster,
    wool=wool}      | _______________________________ |
| {munchkin=blue,
    winkie=yellow,
    corn=yellow,
    grass=green,
    emerald=green}     | _______________________________      |
| {pumpkin=peach,
    corn=apple,
    apple=apple,
    pie=fruit,
    peach=peach} | _______________________________      |
| {lab=IPL,
    lion=cat,
    terrier=dog,
    cat=cat,
    platypus=animal,
    nyan=cat} | _______________________________      |