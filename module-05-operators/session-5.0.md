# C++ Operators
Operators are used to perform operations on variables and values.

- In the example below, we use the + operator to add together two values:

```cpp
int x = 100 + 50;
```

Although the + operator is often used to add together two values, like in the example above, it can also be used to add together a variable and a value, or a variable and another variable:


### Example

```cpp
int sum1 = 100 + 50;        // 150 (100 + 50)
int sum2 = sum1 + 250;      // 400 (150 + 250)
int sum3 = sum2 + sum2;     // 800 (400 + 400)
```


|   Operator    |     Name          |	          Description               |	Example |
|---------------|-------------------|---------------------------------------|-----------|
|   +	        |    Addition	    | Adds together two values	            |   x + y   |	
|   -	        |    Subtraction	| Subtracts one value from another	    |   x - y	|    
|   *	        |    Multiplication	| Multiplies two values	                |   x * y	|    
|   /	        |    Division	    | Divides one value by another	        |   x / y	|
|   %	        |    Modulus	    | Returns the division remainder	    |   x % y	|
|   ++	        |    Increment	    | Increases the value of a variable by 1|	++x	    |
|   --	        |    Decrement	    | Decreases the value of a variable by 1|	--x     |


# C++ Assignement Operator
Assignment operators are used to assign values to variables.

- In the example below, we use the assignment operator (=) to assign the value 10 to a variable called x:

### Example
```cpp
int x = 10;
```

# C++ Comparison Operators

- Comparison operators are used to compare two values (or variables). This is important in programming, because it helps us to find answers and make decisions.

- The return value of a comparison is either 1 or 0, which means true (1) or false (0). These values are known as Boolean values, and you will learn more about them in the Booleans and If..Else chapter.

- In the following example, we use the greater than operator (>) to find out if 5 is greater than 3:

### Example

```cpp
int x = 5;
int y = 3;
cout << (x > y); // returns 1 (true) because 5 is greater than 3
```


|   Operator    |	Name	                    |   Example |
|---------------|-------------------------------|-----------|	
|       ==      |	Equal to	                |   x == y	|
|       !=	    |   Not equal	                |   x != y	|
|       >	    |   Greater than	            |   x > y	|
|       <	    |   Less than	                |   x < y	|
|       >=	    |   Greater than or equal to    |	x >= y	|
|       <=	    |   Less than or equal to	    |   x <= y  |



# C++ Logical Operators
As with comparison operators, you can also test for true (1) or false (0) values with logical operators.

- Logical operators are used to determine the logic between variables or values:

|   Operator    |	Name	    |   Description	                                            | Example	        |
|---------------|---------------|-----------------------------------------------------------|-------------------|
|       && 	    |   Logical and	|Returns true if both statements are true	                | x < 5 &&  x < 10	|
|       \|\|      | 	Logical or	|Returns true if one of the statements is true	            | x < 5 || x < 4	|
|       !       |	Logical not	|Reverse the result, returns false if the result is true	| !(x < 5 && x < 10)|	


    
