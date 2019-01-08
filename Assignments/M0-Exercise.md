## Exercises

The goal for this module is to set up your development environment that will allow you to complete the exercises and try the demos. 

1. Ensure that you have a working version of [Eclipse for Java](http://www.eclipse.org/) and [Java 8](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
2. Install the Checkstyle Eclipse Plug-in. In Eclipse, select `Help | Eclipse Marketplace...` and enter `Checkstyle` in the `Find:` box. From the results, install `Checkstyle Plug-In...`.
3. Similar as the above, install the EclEmma Eclipse-Plug-In. Note that in the more recent versions of Eclipse, it is possible that EclEmma is already installed in the default distribution.
4. Clone the [SoftwareDesignCode](https://github.com/jin-guo/SoftwareDesignCode) project into your Eclipse workspace. In the Eclipse package explorer, right-click and select `Import... | Git -> Projects from Git | Clone URI` and under URI enter `https://github.com/jin-guo/SoftwareDesignCode`, then click-through, requesting to import existing Eclipse projects. Once imported, the project should compile without errors.
5. Just like you did for step 4, clone the [JetUML](https://github.com/prmr/JetUML) project into your Eclipse workspace. For convenience, you can also download the [executable file](http://cs.mcgill.ca/~martin/jetuml/) and place it somewhere convenient.
6. Just like you did for steps 4 and 5, clone the [Solitaire](https://github.com/prmr/Solitaire) project into your Eclipse workspace.

To ensure that everything works:

1. In the SoftwareDesignCode project, in package `...demo`, right-click on the file `Welcome.java` and select `Run As... | Java Application`. You should see a small GUI application appear. Try the different buttons which should do the obvious thing.
2. Right-click on the file `TestAlternatingLabelProvider.java` and select `Run As... | JUnit Test`. A green bar should appear.
3. Right-click again on the file `TestAlternatingLabelProvider.java` and select `Coverage As... | JUnit Test`. A green bar should appear, along with a view showing coverage information. If you go back to the source code file, most lines should be highlighted in green. The meaning of this will be explained in class in a later module.
4. Access the "Problems" view in Eclipse. You should see two warnings of the type "Checkstyle Problem".

Once everything works as described above, try the following:

1. Fix the code to make the Checkstyle warnings go away. To see the full list of coding rules checked by the tool, right-click on the project and select `Properties | Checkstyle | Configure` and play around with the viewer.
2. Change line 37 of file `AlternatingLabelProvider.java` to return `aLabel1` instead of `aLabel2`, and re-run the test. The test should fail.
3. Learn some [seriously useful shortcuts](http://www.vogella.com/tutorials/EclipseShortcuts/article.html).

---
Note: this content is updated from exercises in [Introduction to Software Design with Java](https://github.com/prmr/SoftwareDesign/blob/master/modules/Module-00.md) by Martin P. Robillard