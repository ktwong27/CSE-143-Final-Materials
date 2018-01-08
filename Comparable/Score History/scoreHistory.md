### ScoreHistory


Imagine a video game that produces scores in the range -5 to 5 (5 is the best possible score, 5 is the worst). Players are ranked according to their all-time highest score. If two players have the same all-time high score, the player who has scored the high score the most times is the higher ranked. Two players who have scored the high score an equal number of times are ranked equally.

For example a player scoring (-5, -4, 4, 4) is ranked higher than a player who scores (4, 3, 3, 3) because player 1 has scored 4 two times.

Write a class ScoreHistory that keeps track of player scores in this game. Include the following functionality:

     ScoreHistory(name)                    History should be constructed with a String repre-
                                           senting the player name

    addScore(int)                          takes an integer parameter representing the score (it
                                           should throw an IllegalArgumentException if the score
                                           is not in the range -5 to 5)

    numberOfPlays()                        returns the number of times a score has been recorded

    Comparable                             Your class should also implement the Comparable inter-
                                           face. A ScoreHistory is greater than another if the high
                                           score is greater. If two ScoreHistory objects have the
                                           same high score, ScoreHistory with the greatest number
                                           of that score is greater. If both ScoreHistory objects have
                                           the same number of the high score, they are equal.

You can use any fields you wish in the ScoreHistory. You can also write any helper methods you need to accomplish the described functionality.
