##Chapter 2. Control Structures and Functions

###Answers

1) **Answer**:      

    def signum(x: Int): Int = 
      if (x > 0) 1 
      else if (x < 0) -1 
      else 0
      
2) **Answer**:      

The value of `{}` is `()`, type is `Unit`.



3) **Answer**:      

    var x = ()
    var y = 0
    x = y = 1
    

4) **Answer**:      

    for (i <- 10 to 0 by -1)
      println(i)


5) **Answer**:      

    def countdown(n: Int) = {
      for (i <- n to 0 by -1)
        println(i)
    }
    

6) **Answer**:      

    var acc = 1L
    val word = "Hello"
    for (c <- word)
        acc *= c.toInt
    println(acc)
    

7) **Answer**:      

    val word = "Hello"
    val acc = (1L /: word)(_ * _.toInt)
    println(acc)


8) **Answer**:      

    def product(s: String): Long = (1L /: s)(_ * _.toInt)


9) **Answer**:      

    def product(s: String): Long = 
        if (s.isEmpty) 1L
        else s.head.toInt * product(s.tail)

  
10) **Answer**:      

      def Power(x: Double, n: Int): Double =
        if (n == 0) 1
        else if (n < 0) 1 / Power(x, -n)
        else if (n % 2 == 0) Power(x, n / 2) * Power(x, n / 2)
        else x * Power(x, n - 1)  

