##Chapter 1. The Basics

###Answers

1) In the Scala REPL, type `3.` followed by the Tab key. What methods can be applied?     
**Answer**:

* `%`
* `&`
* `*`
* `+`
* `-`
* `/`
* `>`
* `>=`
* `>>`
* `>>>`
* `^`
* `asInstanceOf`
* `isInstanceOf`
* `toByte`
* `toChar`
* `toDouble`
* `toFloat`
* `toInt`
* `toLong`
* `toShort`
* `toString`
* `unary_+`
* `unary_-`
* `unary_~`
* `|`


2) In the Scala REPL, compute the square root of 3, and then square that value. By how much does the result differ from 3? (Hint: The `res` variables are your friend.)     
**Answer**:

    scala> import scala.math._
    import scala.math._
    
    scala> sqrt(3)
    res0: Double = 1.7320508075688772
    
    scala> pow(res0, 2)
    res1: Double = 2.9999999999999996
    
    scala> 3 - res1
    res2: Double = 4.440892098500626E-16


3) Are the `res` variables `val` or `var`?     
**Answer**:    
`res` is `val` because --

    scala> 77*88
    res0: Int = 6776
    
    scala> res0 = 999
    <console>:8: error: reassignment to val
            res0 = 999
                ^


4) Scala lets you multiply a string with a number—try out `"crazy" * 3` in the REPL. What does this operation do? Where can you find it in Scaladoc?     
**Answer**:      
It repeats the string for given times. e.g.

    scala> "crazy" * 3
    res1: String = crazycrazycrazy
    
Found `def *(n: Int): String` on [StringOps](http://www.scala-lang.org/api/current/index.html#scala.collection.immutable.StringOps)


5) What does `10 max 2` mean? In which class is the max method defined?     
**Answer**:      
`10 max 2` means `10.max(2)`. It's defined in object *math* of *scala.math* package.     


6) Using `BigInt`, compute 2^1024.     
**Answer**:     

    import scala.math._
    BigInt(2).pow(1024)


7) What do you need to import so that you can get a random prime as `probablePrime(100, Random)`, without any qualifiers before `probablePrime` and `Random`?     
**Answer**:     
    
    import scala.math.BigInt._
    import scala.util._
    probablePrime(100, Random)


8) One way to create random file or directory names is to produce a random `BigInt` and convert it to base 36, yielding a string such as `"qsnvbevtomcj38o06kul"`. Poke around Scaladoc to find a way of doing this in Scala.     
**Answer**:     

    import scala.math.BigInt._
    import scala.util._
    probablePrime(1024, Random).toString(36)


9) How do you get the first character of a string in Scala? The last character?     
**Answer**:      
Use `.head` to get the first, and `.last` to get the last.



10) What do the `take`, `drop`, `takeRight`, and `dropRight` string functions do? What advantage or disadvantage do they have over using `substring`?     
**Answer**:     

* `take` : Selects first *n* elements.      
* `drop` : Selects all elements except first *n* ones.     
* `takeRight` : Selects last *n* elements.     
* `dropRight` : Selects all elements except last *n* ones.     







