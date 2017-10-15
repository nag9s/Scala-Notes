Tuples are ordered sets of values; you can think of tuples like records in a table in a relational database, where each element or value can be referenced by position.

The position of the value in the tuple has some relevance, unlike the position of an element in a list. Tuples can contain objects with a mixture of data types. Also like lists, tuples are immutable data structures.

![](/assets/tupleEx.png)

Note in the last example that I used the class name Tuple3; if the tuple contained four elements, I would use the class name Tuple4, and so on.

After you have created a tuple, you can access any of the fields positionally by using \_&lt;field\_no&gt;; unlike lists or arrays, which are zero-based \(meaning 0, 1, 2\), element position in a tuple is one-based \(meaning 1, 2, 3\).



![](/assets/AccessingTuples.png)

