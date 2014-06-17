##Chapter 2. Control Structures and Functions

###Exercises
       
1.	The *signum* of a number is 1 if the number is positive, –1 if it is negative, and 0 if it is zero. Write a function that computes this value.       

2.	What is the value of an empty block expression `{}`? What is its type?       

3.	Come up with one situation where the assignment `x = y = 1` is valid in Scala. (Hint: Pick a suitable type for `x`.)       

4.	Write a Scala equivalent for the Java loop       

        for (int i = 10; i >= 0; i--) System.out.println(i);

5.	Write a procedure `countdown(n: Int)` that prints the numbers from *n* to 0.       

6.	Write a for loop for computing the product of the Unicode codes of all letters in a string. For example, the product of the characters in `"Hello"` is `9415087488L`.       

7.	Solve the preceding exercise without writing a loop. (Hint: Look at the `StringOps` Scaladoc.)       

8.	Write a function `product(s : String)` that computes the product, as described in the preceding exercises.       

9.	Make the function of the preceding exercise a recursive function.       

10.	Write a function that computes x^n, where n is an integer. Use the following recursive definition:       

    * *x^n = y^2* if *n* is even and positive, where *y = x^n / 2*.       
    * *x^n = x·x^(n–1)* if *n* is odd and positive.       
    * *x^0 = 1*.       
    * *x^n = 1 / x^(–n)* if *n* is negative.       
    * Don't use a `return` statement.       

