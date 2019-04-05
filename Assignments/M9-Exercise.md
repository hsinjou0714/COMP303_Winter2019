## Exercises

For maximum learning effectiveness, please check the [answers](../Answers/M9-Answers.md) only after giving the problems an honest try.

1. Write a program where one thread (`NumberIncrementer`) keeps adding to a shared data structure (make it a class `NumberBox`), and another thread (`NumberPrinter`) sleeps, periodically wakes up, and prints whatever number is in the box. Do you need to use synchronization? why or why not?
2. Change the program of Exercise 1 so the number-incrementer threads only increments number every, say, 1 second, and the printer
thread only obtains a number when a new one is available. Use conditions.
3. Enhance the version developed for Exercise 2 so that a third (timer) thread interrupts both counter and printer threads after the number reaches 10.

---
Note: this content is updated from exercises in [Introduction to Software Design with Java](https://github.com/prmr/SoftwareDesign/blob/master/modules/Module-09.md) by Martin P. Robillard