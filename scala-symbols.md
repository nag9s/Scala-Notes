We can divide the operators in Scala, for the purpose of teaching, into four categories:

* Keywords/reserved symbols
* Normal methods or values
* Methods provided by implicit conversion
* Syntactic sugars/composition

And let’s see some arbitrary examples:

![](/assets/symbol.png)

The exact meaning of most of these methods depends on the class they are defined on. For example, `<=` on `Int` means _“less than or equal to”_, but it might mean something else in another class. `::` in an expression is probably the method of the class `List` but it can also refer to the object of the same name \(and in a pattern it definitely does\).

So, let’s discuss these categories.



## Keywords/reserved symbols {#keywordsreserved-symbols}



