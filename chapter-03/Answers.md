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


2) **Answer**:      
    
    import scala.collection.mutable.ArrayBuffer
    
    val a = Array(1, 2, 3, 4, 5)
    
    val tmp = ArrayBuffer[Int]()
    for (i <- 0 until a.length by 2)
      if (i + 1 < a.length) tmp += ( a(i + 1), a(i) )
      else tmp += a(i)
    
    tmp.toArray

