# Scala-Notes

Side Effects -     we will restrict ourselves to constructing programs  
  using only pure functions with **no side effects such as reading from files or mutating memory.**- **Functional Programming in Scala-Manning Publications \(2014\)**

**Functional Programming, Simplified\_ \(Scala edition\) \(2017\)**

in other words, functions that have no side effects.

What are side effects? A function has a side effect if it does something other than simply return a result, for example:

* Modifying a variable
* Modifying a data structure in place
* Setting a field on an object
* Throwing an exception or halting with an error
* Printing to the console or reading user input
* Reading from or writing to a file

## 

**Functional Programming, Simplified\_ \(Scala edition\) \(2017\)**

The answer is that you violate the “Write Only Pure Functions” rule! It seems like  
 many other resources go through great lengths to avoid answering that question, but I  
 just gave you that answer fairly early in this book. \(You’re welcome.\)

The general idea is that you write as much of your application as possible in an FP  
 style, and then handle the UI and all forms of input/output \(I/O\) \(such as Database  
 I/O, Web Service I/O, File I/O, etc.\) in the best way possible for your current  
 programming language and tools.

In Scala the percentage of your code that’s considered impure I/O will vary,  
 depending on the application type, but will probably be in this range:

1. On the low end, it will be about the same as a language like Java. So if you
    were to write an application in Java and 20% of it was going to be impure I/O
    code and 80% of it would be other stuff, in FP that “other stuff” will be pure
   functions. This assumes that you treat your UI, File I/O, Database I/O, Web
    Services I/O, and any other conceivable I/O the same way that you would in
    Java, without trying to “wrap” that I/O code in “functional wrappers.” \(More on
    this shortly.\)
2. On the high end, it will approach 100%, where that percentage relies on two
    things. First, you wrap all of your I/O code in  unctional wrappers. Second,
    your definition of “pure function” is looser than my definition.

The return values of expressions will be passed to other expressions or storedinto values.

As you migrate from using variables, your functions and expressions willhave fewer side effects. In other words, they will purely act on the input you give themwithout affecting any data other than their return value. This is one of the main goalsand benefits of functional programming.

