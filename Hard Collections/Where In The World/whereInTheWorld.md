<div class="viewer">

### whereInTheWorld

<div>

Write a method named whereInTheWorld that accepts two parameters:

1.  a String representing the name of a person

2.  a Map in which keys represent names of cities and values represent the set of which friends have visited the city

Your method should return a set of the cities where the given person has been. The set returned should be sorted alphabetically.

For example, given the following map called places:

    {"Joe"=["New York", "San Francisco"], "Samantha"=["London"],
     "Elias"=["London", "New York", "San Francisco", "Singapore"],
     "Myra"=["Beijing", "Beirut", "Nashville", "Phoenix"]}

The call to whereInTheWorld("New York", places) should return the set:

    ["Joe", "Elias"]

because Joe and Elias have visited New York.

Your method should return only names that match the city exactly, including case. Your method should not modify the contents of the map. You may assume that the map passed to your method is not null and that it does not contain any null values.

</div>

</div>