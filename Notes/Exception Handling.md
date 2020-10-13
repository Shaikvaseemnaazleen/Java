# Exception-Handling 

* An exception is an event, which occurs during the execution of a program, that disrupts the normal flow of the program's instructions.
* When an exceptional condition arsies, an object representing that exception is created and thrown in the method that caused the error.
* Exceptions can be generated by java run-time system, or they can be manually generated by your code.
  * Exceptions thrown by Java relate to fundamental errors that violate the rules of the java language or the
    constraints of the java execution
  * Manually generated exceptions are typically used to report some error condition to the caller of the method.
  

## Types of Exceptions
 ### Checked exceptions
 * Checked exceptions are exceptional conditions that a well-written application should anticipate and recover from.
 * Checked exceptions are subject to the Catch or Specify Requirement.
 * All exceptions are checked exceptions, except for those indicated by Error, RuntimeException, and their subclasses.
 ### Unchecked exceptions
 Errors and runtime exceptions are collectively known as unchecked exceptions.
   #### Error
  * These are exceptional conditions that are external to the application, and that the application usually cannot        anticipate or recover from
  * Errors are not subject to the Catch or Specify Requirement
  * Errors are those exceptions indicated by Error and its subclasses.
   #### Runtime exceptions
  * These are exceptional conditions that are internal to the application, and that the application usually cannot     anticipate or recover from
  * These usually indicate programming bugs, such as logic errors or improper use of an API
  * Runtime exceptions are not subject to the Catch or Specify Requirement
  *  Runtime exceptions are those indicated by RuntimeException and its subclasses.


## Keywords

* Java Exceptions are handled by 5 keywords:
   * try
   * catch
   * throw
   * throws
   * finally

* Program statements that want to be monitored for exceptions are contained within a **try** block. If an exception occurs in try block, it is thrown.
* If an exception occurs in the try block, it is thrown, we can catch this exception using **catch** and handle in some rationak manner.
* To manually throw exception, use the keyword **throw**.
* Any exception that is thrown out of a method must be specified as such by a **throws** clause.
* Any code that absolutely must be executed after a **try** block completes is put in a **finally** block.

## Syntax

```
try {
  // block of code to monitor for errors
}
catch (ExceptionType1 exOb) {
  // exception handler for ExceptionType1
}
catch (ExceptionType2 exOb) {
  // exception handler for ExceptionType2
}
  
// ...

finally {
  // block of code to be executed after try block ends
}
```

## try-catch

```
try {
  // block of code to monitor for errors
}
catch (ExceptionType exOb) {
  // exception handler for ExceptionType
}
```

## throw

It is possible for your program to throw an exception explicitly, using the throw
statement

```
throw ThrowableInstance;
```
