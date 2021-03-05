# Test Factorial

This exercise is about getting familiar with unit testing and JUnit 5 approach in particular.

Design and code a `factorial` method in the [Factorial](src/main/java/com/epam/rd/autotasks/Factorial.java) class. Here are some details:

- The method takes a String as a parameter, transforms it to an integer value, and counts its factorial.
- The method returns a result as a String.
- The string parameter `n` must represent a non-negative integer number. If it does not, throw an IllegalArgumentException.

Complete the test classes:


FactorialCsvParametrizedTesting  – 
FactorialMethodSourceParametrizedTesting  – 

- [FactorialBadInputTesting](src/main/java/com/epam/rd/autotasks/FactorialBadInputTesting.java)\
  There are four empty methods that you must complete:
    - `testNullInput` - test null input cases
    - `testNegativeInput` - test negative number input cases
    - `testFractionalInput` - test fractional cases
    - `testNonDigitalInput` - test non-digit cases
- [FactorialCsvParametrizedTesting](src/main/java/com/epam/rd/autotasks/FactorialCsvParametrizedTesting.java)\
  It is a parameterized test that takes arguments from the [csvCases.csv](src/main/resources/csvCases.csv) file.
  Do not change the csv file, only implement the method.
- [FactorialMethodSourceParametrizedTesting](src/main/java/com/epam/rd/autotasks/FactorialMethodSourceParametrizedTesting.java)\
  It is a parameterized test that takes arguments from the `testCases` method.
  Complete the test method and introduce the method that provides the following cases:
    - "1", "1"
    - "2", "2"
    - "5", "120"
- [FactorialRegularInputTesting](src/main/java/com/epam/rd/autotasks/FactorialRegularInputTesting.java)\
  It is a test class where you can add regular test cases.
  Consider covering the cases that are not present in other test classes.
  
To pass the exercise, your tests must correctly detect flaws of some other implementations. 
There are special tests in several classes that apply your tests to your implementation and other problematic (“bad”) ones:
- [FactorialTestingsTest](src/test/java/com/epam/rd/autotasks/FactorialTestingsTest.java)
- [LazyFactorialTestingsTest](src/test/java/com/epam/rd/autotasks/LazyFactorialTestingsTest.java)
- [WrongOperationConcatIntFactorialTestingsTest](src/test/java/com/epam/rd/autotasks/WrongOperationConcatIntFactorialTestingsTest.java)
- [WrongOperationSumIntFactorialTestingsTest](src/test/java/com/epam/rd/autotasks/WrongOperationSumIntFactorialTestingsTest.java)

Your solution method must pass your tests while other implementations must fail your tests in some cases.

Also, there is one more secret test class that you do not have access to. It will be applied to your solution once you submit it to Autocode. So, consider the variety of possible cases.

Hint: [Factorial reference](https://en.wikipedia.org/wiki/Factorial)