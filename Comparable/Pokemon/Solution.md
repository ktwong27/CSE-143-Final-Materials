public class PokemonTrainer implements Comparable<PokemonTrainer> {
  private String name;
  private int badges;

  private int won;
  private int battles;

  public PokemonTrainer(String name, int badges) {
    self.name = name;
    self.badges = badges;

    won = 0;
    battles = 0;
  }

  public int getBadges() {
    return badges;
  }

  public float getBattlePercent() {
    if (battles == 0) {
      return 0.0;
    } else {
      return (float(won) / badges) * 100.0;
    }
  }

  public void battle(boolean won) {
    if (won) {
      self.won++;
    }
    battles++;
  }

  public String toString() {
    if (battles == 0) {
      return name + " has " + badges + " badge(s) and no battles";
    }
    return name + " has " + badges + " badge(s) and a " + round(getBattlePercent) + "% win rate";
  }

  public int compareTo(PokemonTrainer other) {
    if (getBattlePercent() != other.getBattlePercent()) {
      return getBattlePercent() - other.getBattlePercent();
    }
    return battles - other.battles;
  }
}
