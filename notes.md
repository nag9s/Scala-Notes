![](/assets/notes1.png)

Look in the above, just not including \(\) , scala complaints about an error - missing paramater type, so , be careful with invoking functions.

1. Scala allows the omission of parentheses on methods of arity-0 \(no arguments\):

reply\(\)

// is the same as

reply

However, this syntax should \_only \_be used when the method in question has no side-effects \(purely-functional\). In other words, it would be acceptable to omit parentheses when calling `queue.size`, but not when calling `println()`. This convention mirrors the method declaration convention given above.

[https://docs.scala-lang.org/style/method-invocation.html](https://docs.scala-lang.org/style/method-invocation.html)

And also more details @ scala impatient ch 5.1

