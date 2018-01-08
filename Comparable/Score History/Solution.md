public class ScoreHistory implements Comparable<ScoreHistory> {
  private String name;
  private int highScore;
  private int count;
  private int total;

  public ScoreHistory(String name) {
    self.name = name;
    highScore = -6;
    count = 0;
    total = 0;
  }

  public void addScore(int score) {
    if (score < -5 || score > 5) {
      throw new IllegalArgumentException();
    }
    total++;
    if (score > highScore) {
      highScore = score;
    }
    if (score == highScore) {
      count++;
    }
  }

  public func numberOfPlays() {
    return total;
  }

  public int compareTo(ScoreHistory other) {
    if (highScore != other.highScore) {
      return other.highScore - highScore;
    } else {
      return other.count - count;
    }
  }

}
