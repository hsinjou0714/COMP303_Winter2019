## Exercises

For maximum learning effectiveness, please check the [answers](../Answers/M5-Answers.md) only after giving the problems an honest try.

1. Draw a UML Sequence Diagram to represent the following program. Consider that the `main` method can be approximated as an object with name `client`:

```java
public static void main(String[] args)
{
   String string1 = "Foo";
   String string2 = "Bar";
   System.out.println(string1.compareTo(string2));
}
```

2. Study the code of method [`GameModel.undoLast()`](https://github.com/prmr/Solitaire/blob/master/src/ca/mcgill/cs/stg/solitaire/model/GameModel.java#L239) in the Solitaire application and create a UML sequence diagram to model the key object interactions in this method. Note that this and similar code exploration questions will be much easier and more enjoyable to complete using a clone of the project workspace.

3. Make the [Hand](https://github.com/jin-guo/SoftwareDesignCode/blob/master/module02/ca/mcgill/cs/swdesign/m2/Hand.java) class cloneable. Write a small driver program that creates a new `Hand` object and clones it. Create a UML object diagram to represent a cloned Hand. Use the debugger to verify the correctness of your diagram.

4. Starting from the [Module 5 Code Samples](https://github.com/jin-guo/SoftwareDesignCode/blob/master/module05/ca/mcgill/cs/swdesign/m5), implement method `clone` in class `ConferenceShow`.

5. Starting from the [Module 5 Code Samples](https://github.com/jin-guo/SoftwareDesignCode/blob/master/module05/ca/mcgill/cs/swdesign/m5), enhance the design with the concept of a composite command, and use this feature to implement a command that clears the program and adds one show to the fresh program.

6. Starting from the [Module 5 Code Samples](https://github.com/jin-guo/SoftwareDesignCode/blob/master/module05/ca/mcgill/cs/swdesign/m5), enhance the design with the concept
of a "logged command" that logs any kind of command to the console after having executed it. 

7. Design a `CompositeIcon` class that can contain multiple icons. Note that a standard application of the Composite design pattern will result in the composed icons being painted on top of each other. Solve this problem with a `ShiftedIcon` decorator that will support drawing an icon as shifted by (parametric) x and y values. Extend the following diagram to complete the design. Make sure you list all the methods (including constructors) that will be necessary to make this work.

![](m05-exercise7.png)

8. Draw a sequence diagram showing what happens to a composite icon after a paintIcon callback.

9. Implement the solution using the [module's source code samples](https://github.com/jin-guo/SoftwareDesignCode/blob/master/module05/ca/mcgill/cs/swdesign/m5/icon) as a template. When you solve this exercise, executing the main method of the `BridgeDealer` class should show a graphical window where card icons are laid out according to your solution.

## Optional
The following exercises are are optional. The ones prefixed with :star: are more challenging questions aimed to provide you with additional design and programming experience. The ones prefixed with :spades: will incrementally guide you towards the ultimate completion of a complete Solitaire application.

1. :star: Write unit tests for the `getIconHeight()` and `getIconWidth()` method using stubs.

2. :spades: Study the code of the [Solitaire](https://github.com/prmr/Solitaire/blob/master/src/ca/mcgill/cs/stg/solitaire/model/) application and draw a UML class diagram that shows how the Command design pattern is used to support game `Move`s.

---
Note: this content is updated from exercises in [Introduction to Software Design with Java](https://github.com/prmr/SoftwareDesign/blob/master/modules/Module-05.md) by Martin P. Robillard