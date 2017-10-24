you can think of the =&gt; symbol as a transformer. In this case, the function transforms the Int value i to an Int value that is twice the value of i.

`(i: Int) => { i * 2 }`

You can now assign that function literal to a variable:

`val double = (i: Int) => { i * 2 }`

The variable double is an instance, just like an instance of a String, Int, or other type,  but in this case, it’s an instance of a function, known as a function value. You can now  invoke double just like you’d call a method:

`double(2) // 4`

`double(3) // 6`

