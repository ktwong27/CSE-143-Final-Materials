<div class="viewer">

### convertNames

<div>

Write a method called convertNames that takes as a parameter a list of strings representing names and that returns a map of strings to sets of strings that represent the same names split into first and last names. In particular, the names in the list passed to the method will each include a last name followed by a single comma and a space followed by the first name. You are guaranteed that there are no other commas in the string.

    [“Monroe, James”, “Madison, James”, “Adams, John”, “Tyler, John”, “Van Buren,
     Martin”, “Jackson, Andrew”]

The method should split each string into the last name that comes before the comma and the space, and the first name that comes after. The method should construct and return a map in which the keys are the first names and the values are the set of last names that match the first names.

For the list of names above, the following map would be constructed:

    {“Andrew”=[“Jackson”], “James”=[“Madison”, “Monroe”], “John”=[“Adams”, “Tyler”],
     “Martin”=[“Van Buren”]}

Notice, for example, that two of the names in the original list have “John” as the first name. In the map, the key "John" maps to a set of two elements (the two last names connected to “John”).

Your method should construct the new map and each of the sets contained in the map. Recall that the String class has a substring method that takes a starting index (inclusive) and a stopping index (exclusive). For example:

    "Australia".substring(1, 5) returns "ustr"

The keys of the new map should be ordered alphabetically by the first names and each set should be ordered alphabetically by the last names contained in the set.

</div>

</div>