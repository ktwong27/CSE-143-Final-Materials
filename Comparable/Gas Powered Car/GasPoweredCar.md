<div class="viewer">

### GasPoweredCar

<div>

Define a class GasPoweredCar that keeps track of information about the fuel efficiency of various types of cars. Each GasPoweredCar object keeps track of model name, along with its advertised miles per gallon, and the amount of gas (in gallons) that its tank can hold. The class has the following public methods:

     GasPoweredCar(model, mpg,      Constructs a Car object with the given
                   fuelCapacity)    model name and the given miles per gallon
                                    and gas tank capacity. 

     getModel()                     Returns the model name.

     calcRange()                    Returns the total number of miles the
                                    car can travel on one tank of gasoline.

     toString()                     Returns a String with model name, 
                                    miles per gallon, and fuel capacity.

    GasPoweredCar car1 = new GasPoweredCar("Toyota Prius", 50, 11.9, 23000);
    GasPoweredCar car2 = new GasPoweredCar("Ferrari F430", 13, 25.1, 188000);
    GasPoweredCar car3 = new GasPoweredCar("Hummer H3 SUV", 15, 23.0, 34000);
    GasPoweredCar car4 = new GasPoweredCar("Honda Accord", 25, 18.5, 29000);

So car1 represents a Toyota Prius, which is advertised as getting 50 miles per gallon, and has a gas tank that will hold 11.9 gallons. Miles per gallon will only be given as an integer, but fuelCapacity can be a real number. Your constructor should throw an IllegalArgumentException if any of the numeric values passed to it is negative.

This class is being used by a program that allows potential car buyers to find cars with the highest miles per gallon and range.

To compute the total number of miles the car can travel on one tank of gasoline, you should multiply miles per gallon (mpg) times the gas tank capacity (fuelCapacity).

    car1.calcRange(); // should return 50 * 11.9 = 595.0
    car2.calcRange(); // should return 13 * 25.1 = 326.3

The toString method should include the model name followed by the miles per gallon and fuel capacity in parenthesis as shown below for car1 and car2.

    Toyota Prius (50 mpg, fuel capacity: 11.9 gallons)
    Ferrari F430 (13 mpg, fuel capacity: 25.1 gallons)

Your toString method must exactly reproduce this format.

The GasPoweredCar class should implement the Comparable<span></span> interface. Cars should be ordered first by miles per gallon. Cars with higher miles per gallon should be considered to be "less" than other cars so that they appear at the beginning of a sorted list. If two cars have the same miles per gallon, then they should be sorted by range. Again, a larger range is considered better and should come first. Finally, if mpg and range are the same, then sort alphabetically by model name.

You may assume that all values passed to your methods are valid and that the total number of problems is greater than 0.

</div>

</div>