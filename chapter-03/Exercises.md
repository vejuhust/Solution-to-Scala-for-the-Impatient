##Chapter 3. Working with Arrays

###Exercises
       
1.	Write a code snippet that sets *a* to an array of *n* random integers between *0* (inclusive) and *n* (exclusive).       

2.	Write a loop that swaps adjacent elements of an array of integers. For example, `Array(1, 2, 3, 4, 5)` becomes `Array(2, 1, 4, 3, 5)`.       


3.	Repeat the preceding assignment, but produce a new array with the swapped values. Use `for`/`yield`.       


4.	Given an array of integers, produce a new array that contains all positive values of the original array, in their original order, followed by all values that are zero or negative, in their original order.       


5.	How do you compute the average of an `Array[Double]`?       


6.	How do you rearrange the elements of an `Array[Int]` so that they appear in reverse sorted order? How do you do the same with an `ArrayBuffer[Int]`?       


7.	Write a code snippet that produces all values from an array with duplicates removed. (Hint: Look at Scaladoc.)       


8.	Rewrite the example at the end of Section 3.4, “Transforming Arrays,” on page 32. Collect indexes of the negative elements, reverse the sequence, drop the last index, and call `a.remove(i)` for each index. Compare the efficiency of this approach with the two approaches in Section 3.4.       


9.	Make a collection of all time zones returned by `java.util.TimeZone.getAvailableIDs` that are in America. Strip off the `"America/"` prefix and sort the result.       


10.	Import `java.awt.datatransfer._` and make an object of type `SystemFlavorMap` with the call       

        val flavors = SystemFlavorMap.getDefaultFlavorMap().asInstanceOf[SystemFlavorMap]

