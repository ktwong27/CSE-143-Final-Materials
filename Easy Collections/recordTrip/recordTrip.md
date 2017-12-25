<html><head>
    <title>recordTrip</title>
    <meta charset="utf-8">
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css" integrity="sha384-1q8mTJOASx8j1Au+a5WDVnPi2lkFfwwEAa8hDDdjZlpLegxhjVME1fgjWPGmkzs7" crossorigin="anonymous">
  <style></style></head>
  <body><div class="viewer"><h3>recordTrip</h3><div><p>Write a method called recordTrip that records information about trips taken by people.  Trip information will be stored in a map in which the keys are names of people and the values are sets of place names.  The method will take as parameters the map followed by a person's name followed by a place name.  For example, if we start with an empty map stored in a variable called trips and we make the following calls:</p><pre><code>recordTrip(trips, "John", "London");
recordTrip(trips, "Sally", "Seattle");
recordTrip(trips, "John", "Paris");
recordTrip(trips, "Sally", "San Francisco");
recordTrip(trips, "John", "NYC");
recordTrip(trips, "John", "Paris");
</code></pre><p>the map would store the following values after these calls:</p><pre><code>{John=[London, NYC, Paris], Sally=[San Francisco, Seattle]}
</code></pre><p>Notice that the map needs to construct a set for each person to store the names of the places they have visited.  The sets it constructs should store the place names in alphabetical order.  You may construct iterators and the sets that store place names, but you are not allowed to construct other structured objects (no string, set, list, etc.).</p></div></div>
</body></html>