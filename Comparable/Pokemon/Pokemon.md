### PokemonTrainer


Define a class PokemonTrainer that stores information about a Pokemon trainer and how many battles they have won. Each PokemonTrainer object keeps track of a trainer's name, number of badges, total battles played, and number of battles won.

The class has the following public methods:

    PokemonTrainer(name, badges)     constructs a PokemonTrainer object with the given
                                     name and number of badges. When a PokemonTrainer
                                     object is constructed, it has played zero battles.

    getBadges()                      returns the number of badges the trainer has earned

    getBattlePercent()               returns a real number representing the exact percent
                                     of battles this trainer has won. If the trainer has
                                     won all of their battles, should return 100.0, if the
                                     trainer has won none of their battles, should return
                                     0.0\. If the trainer has not played any battles yet,
                                     should return 0.0

    battle(boolean won)              records a battle for this trainer. Passed true if
                                     the trainer won the battle, false otherwise

    toString()                       returns a String with name, number of badges, and
                                     percent of wins (or "no battles" if none). The battle
                                     percentage should be truncated after the decimal,
                                     so if getBattlePercent() returned 73.835, then
                                     toString would report a battle percent of 73%

Below is example client code using PokemonTrainer objects:

    PokemonTrainer trainer1 = new PokemonTrainer("Riley", 1);
    PokemonTrainer trainer2 = new PokemonTrainer("Melissa", 6);

    trainer2.getBadges()          // returns 6
    trainer1.battle(true)         // records a battle win for trainer1
    trainer1.battle(false)        // records a battle loss for trainer1
    trainer1.getBattlePercent()      // returns 50.0
    trainer2.getBattlePercent()      // returns 0.0
    trainer1.battle(false)        // records a battle loss for trainer1
    trainer1.getBattlePercent()      // returns 33.3333333333333333
    trainer1.toString()        // returns "Riley has 1 badge(s) and a 33% win rate"
    trainer2.toString()        // returns "Melissa has 6 badge(s) and no battles"

The PokemonTrainer class should be comparable to other PokemonTrainer objects and should implement the Comparable interface. Trainers that have a higher battle percentage should be considered "less" than other trainers so that they appear at the beginning of a sorted list. You should use the complete value of the battle percentage rather than a truncated value. Trainers that have the same battle percentage should be ordered by the number of battles played, with trainers who have battled more often considered "less" than trainers that have battled less frequently.
