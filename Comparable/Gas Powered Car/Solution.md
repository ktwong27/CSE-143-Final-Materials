public class GasPoweredCar implements Comparable<GasPoweredCar> {

  private String model;
  private float mpg;
  private float fuelCapacity;

  public GasPoweredCar(String model, float mpg, float fuelCapacity) {
    self.model = model;
    self.mpg = mpg;
    self.fuelCapacity = fuelCapacity;
  }

  public String getModel() {
    return model;
  }

  public float calcRange() {
    return mpg * fuelCapacity;
  }

  public String toString() {
    return model + " (" + mpg + " mpg, fuel capacity: " + fuelCapacity + " gallons";
  }

  public int compareTo(GasPoweredCar other) {
    if (mpg != other.mpg) {
      if (other.mpg > mpg) {
        return -1;
      }
      return 1;
    } else if (range != other.range) {
      if (other.range > range) {
        return -1;
      }
      return 1;
    } else {
      model.compareTo(other.model);
    }
  }
}
