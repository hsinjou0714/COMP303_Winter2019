## Exercises

For maximum learning effectiveness, please check the [answers](../Answers/M7-Answers.md) only after giving the problems an honest try.

1. A bike courier company uses a Scheduler system to schedule bikers for delivery based on various factors (unimportant for this practice question). The company wants the flexibility to install different scheduling algorithms. However, all scheduling algorithms should follow these steps: (a) check if at least one biker is available, and if not throw an exception; (b) schedule a biker using a given algorithm; (c) notify interested observers that a biker was scheduled. Operations (a) and (c) are the same for all algorithms, but should be isolated in separate methods. Concrete schedulers should also have the flexibility to throw algorithm-specific types of exceptions if they cannot fulfill a scheduling request. Assume all exceptions for this design are checked. Use the TEMPLATE METHOD design pattern to provide a design for these requirements. Also include the OBSERVER mechanism for biker notification. Draw the UML class diagram to illustrate your design. When relevant to the design, make sure to include the appropriate modifiers for methods and/or classes (`final`, `public`, `protected`,`private`, `abstract`, etc.). Write the code necessary to implement the relevant parts of your design.

2. Extend the code of the [LuckyNumber](https://github.com/prmr/SoftwareDesignCode/tree/master/module06/ca/mcgill/cs/swdesign/m6/LuckyNumber.java) sample application to include a Roman Numerals panel.

3. Re-write the code of the [LuckyNumber](https://github.com/prmr/SoftwareDesignCode/tree/master/module06/ca/mcgill/cs/swdesign/m6/LuckyNumber.java) sample application so that data flows between
the model and the observers using the pull strategy. Create a class diagram and a sequence diagram that model the key aspects of this solution.

4. Write the code that implements a skeleton application that corresponds to the Observer Design Case Study. Write a driver program that adds and removes item to make sure everything works as expected. 

5. Study the code of the [Solitaire](https://github.com/prmr/Solitaire) application to see how the `GameModelListener` interface is used. Create a class diagram and a sequence diagram to document how the observer pattern is used in relation to the `GameModel` class.

6. Write a JavaFX application with a button and a label, which writes the current date and time in the label every time the button is pressed. You can obtain the current date and time with the following API call `LocalDateTime.now().toString();`

7. Re-write the code of the [LuckyNumber](https://github.com/prmr/SoftwareDesignCode/tree/master/module06/ca/mcgill/cs/swdesign/m6/LuckyNumber.java) sample application to add a "Notify" button that notifies observers of the value in the model. The value should only be propagated when the button is clicked. 

8. Study the code of the [Solitaire](https://github.com/prmr/Solitaire) application to see how the `DiscardPileView` relies on the observer design pattern to respond to GUI events, and also updates to the model. Draw a class diagram and a sequence diagram to capture the information you discover.
---
Note: this content is updated from exercises in [Introduction to Software Design with Java](https://github.com/prmr/SoftwareDesign/) by Martin P. Robillard