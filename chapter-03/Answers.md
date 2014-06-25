##Chapter 3. Working with Arrays      

###Answers

1) **Answer**:      
    
    import scala.util._
    import scala.collection.mutable.ArrayBuffer
    
    val n = 10
    
    val tmp = ArrayBuffer[Int]()
    for (i <- 0 until n) 
      tmp += Random.nextInt(n)
    
    val a = tmp.toArray

