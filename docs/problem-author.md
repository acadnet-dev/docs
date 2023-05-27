# So you want to create a problem?

## Problem types
Current implemented problem types:
* SimpleAcadnetIS - a simple problem that requires a single .cpp file to be submitted. The file will be compiled and then the tests will be run against it.

## To define a new problem type
#### `Web` project
* Create the new type in `ProblemType` enum
* Create new implementation of `IProblemService` interface and add it to the `ProblemServiceFactory` class

#### `Checker` project
* Add support for the new problem type