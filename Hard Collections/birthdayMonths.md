<div class="viewer">

### birthdayMonths

<div>

Write a method birthdayMonths that accepts as a parameter a map which associates people’s names with their birthdays and returns a map which associates month names to sets of people with birthdays in that month. In the original map, birthdays are represented by Date objects that have day, month and year fields. A Date object’s toString returns a date in month/day/year format. For example, a Date object printed as "12/11/1973" represents December 11th, 1973.

For example, if a map called birthdays contains the following values:

    {Dante Smith=12/11/1973, Lauryn Hill=5/26/1975, Juaqin Maphurs=5/31/1986, Christopher 
     Wallace=5/21/1972, Onika Maraj=12/8/1982, Sean Combs=11/4/1969}

Then the call on birthdayMonths(birthdays) should return the following map:

    {December=[Dante Smith, Onika Maraj], May=[Christopher Wallace, Juaqin Maphurs, Lauryn Hill], 
     November=[Sean Combs]}

Notice that both the months and the names are sorted in alphabetical order. Your method should construct the new map and each of the sets contained in the map but should not construct any other data structures. It should also not modify the map passed as a parameter. You may assume that the map passed in is not null and that it does not contain null values.

The Date class has the following public getters:

*   getDay() – returns an int representing the day of the month of this date
*   getMonth() – returns a String representing the name of the month of this date
*   getYear() – returns an int representing the year of this date

</div>

</div>