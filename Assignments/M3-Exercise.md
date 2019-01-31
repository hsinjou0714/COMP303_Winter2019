## Exercises

For maximum learning effectiveness, please check the [answers](../Answers/M3-Answers.md) only after giving the problems an honest try.

1. Create a UML State Diagram that models the abstract states of a hypothetical `Dryer` object that behaves as follows. *The dryer is normally off. To get it to operate you have to put in 2.00$. Once the money is inserted, you cannot add additional credit until the drying is over. The mechanism to insert the money only allows you to put the exact amount in one go. To start the machine once the money is inserted, you have to close the door and press the start button. The dryer will then operate for exactly 60 minutes, and then stop by itself. If you open the door while it’s in operation, the dryer will stop and whatever time was left is lost.*

2. Create a UML State Diagram that models the abstract states of a hypothetical `VendingMachine` object that behaves as follows. *The machine sells a selection of different drinks. All drinks have a price, not necessarily the same. If a user selects a drink, the price is displayed. If the user adds enough coins within 60 seconds, the drink is provided and change is returned. If a user adds coins without selecting a drink, the available balance is shown. If a user selects a drink that is worth less than the balance, the drink is provided and changed is returned. If not, an error message shows "insufficient balance". A reset button resets any selection and returns the balance.*

3. Change the design of your `Card` class to ensure the uniqueness of its instances through the use of the Flyweight Design Pattern.

## Optional
The following exercises are are optional. The ones prefixed with :star: are more challenging questions aimed to provide you with additional design and programming experience. The ones prefixed with :spades: will incrementally guide you towards the ultimate completion of a complete Solitaire application.

1. :spades: Design and implement a class `WorkingStack` that manages the state of one of the working stacks in Solitaire. Note that as opposed to the `SuitStack` designed in Module 2, for `WorkingStack` you have to solve the problem of remembering which card is visible (or face up), and which card is not.

2. :spades: Using the Singleton Design Pattern, design a `GameModel` class that is a Singleton.

3. :spades: Complete the design of the `GameModel` class. This class will be responsible for managing all the necessary state for a game of solitaire. The class should offer the following state-changing services (through methods): `reset()` initializes a new game by clearing all the working stacks, shuffling the deck, and placing cards on the working stack according to the rules of solitaire (one card on the first stack, two on the second, etc., with the top card of each stack visible); `move(Card, Location)` Moves a card from an assumed legal playing position to the specified location (to be designed); `discard` Moves a card from the top of the deck to the top of the discard pile. In addition, the `GameModel` should provide all the necessary state-querying services, including methods to check the state of the deck and the discard pile (empty or nor), view the cards in the different stacks, etc. In particular, the `GameModel` class should provide a method `getScore()` that returns the cumulative number of cards in the four suit stacks. A score of 52 indicates a win.

4. :spades: Create a UML Class diagram that illustrates the most important elements of your implementation of the `GameModel` class.

5. :spades: Create a UML State diagram that captures all the main abstract states of an instance of the `GameModel` class, and the transitions between them; 

6. :spades: Using the Strategy Design Pattern, add an `autoplay()` method to the `GameModel`, whose purpose is to automatically perform a legal move, if possible. Carefully consider how the strategy should work (inputs, outputs). Consider using the interface segregation principle to decouple the strategy from the `GameEngine`.

7. :spades: :star: Implement, in a main method somewhere (where?), a small driver program that automatically plays N games and reports the average final score per game and the percentage of games won.

---
Note: this content is updated from exercises in [Introduction to Software Design with Java](https://github.com/prmr/SoftwareDesign/blob/master/modules/Module-03.md) by Martin P. Robillard
