Maven, Spring and Eclipse IDE example
=====================================

Let's take by example a Java Spring application, developed in Eclipse IDE.

Global .gitignore
-----------------

The Eclipse IDE is a personal preference of the developer and we cannot assume everyone will be using this IDE. In this case, we PREFER to add Eclipse project files in the global gitignore. Add the following lines to your global .gitignore.
```
.project
.classpath
```
(More gitignore files for Eclipse can be found here [https://github.com/github/gitignore/blob/master/Global/Eclipse.gitignore](https://github.com/github/gitignore/blob/master/Global/Eclipse.gitignore)).

Repository .gitignore
---------------------

Maven will compile files in the `target` directory of the repository. We DON'T want this files to be part of our repository, so add a line in the .gitignore of this repository.
```
target
```

Repository .git/info/exclude
----------------------------

Spring provides Spring Loaded, a JVM agent that allow reloading of classes when a JVM is already running. A developer may want to use spring loaded jar as part of the development in this project but don't want this file to be in the repository. As this is a exclusive case for this project, a entry on the `.git/info/exclude` of the local repository should be added.
```
springloaded-*.jar
```
