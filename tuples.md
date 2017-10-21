Tuples are ordered sets of values; you can think of tuples like records in a table in a relational database, where each element or value can be referenced by position.

gives you a way to store a group of heterogeneous items in a container. Create a tuple by enclosing the desired elements between parentheses. This is a two element tuple:

`scala> val d = ("Debi", 95)`

`d: (String, Int) = (Debi,95)`



scala&gt; case class Person\(name: String\)

defined class Person

scala&gt; val t = \(3, "Three", new Person\("Al"\)\)

t: \(Int, java.lang.String, Person\) = \(3,Three,Person\(Al\)\)



The position of the value in the tuple has some relevance, unlike the position of an element in a list. Tuples can contain objects with a mixture of data types. Also like lists, tuples are immutable data structures.

![](/assets/tupleEx.png)

Note in the last example that I used the class name Tuple3; if the tuple contained four elements, I would use the class name Tuple4, and so on.

After you have created a tuple, you can access any of the fields positionally by using \_&lt;field\_no&gt;; unlike lists or arrays, which are zero-based \(meaning 0, 1, 2\), element position in a tuple is one-based \(meaning 1, 2, 3\).

![](/assets/AccessingTuples.png)

Tuples can be embedded in other types; for instance, it is sometimes useful to have a list of tuples or an

array of tuples.

