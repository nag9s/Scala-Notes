![](/assets/notes1.png)

Look in the above, just not including \(\) , scala complaints about an error - missing paramater type, so , be careful with invoking functions.

1. Scala allows the omission of parentheses on methods of arity-0 \(no arguments\):

reply\(\)

// is the same as

reply

However, this syntax should \_only \_be used when the method in question has no side-effects \(purely-functional\). In other words, it would be acceptable to omit parentheses when calling `queue.size`, but not when calling `println()`. This convention mirrors the method declaration convention given above.

[https://docs.scala-lang.org/style/method-invocation.html](https://docs.scala-lang.org/style/method-invocation.html)

And also more details @ scala impatient ch 5.1

If you include the parentheses in the definition you can optionally omit them when you call the method. If you omit them in the definition you can't use them when you call the method.

[https://stackoverflow.com/questions/7409502/what-is-the-difference-between-def-foo-and-def-foo-in-scala](https://stackoverflow.com/questions/7409502/what-is-the-difference-between-def-foo-and-def-foo-in-scala)

You can call a parameterless method \(such as current\) with or without  
 parentheses:

myCounter.current // OK

myCounter.current\(\) // Also OK

**Which form should you use?** It is considered good style to use \(\) for a  
 mutator method \(a method that changes the object state\), and to drop the \(\)  
 for an accessor method \(a method that does not change the object state\).



Scala By Example

![](/assets/param1.png)

