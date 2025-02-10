### 5.1 Strings Introduction

1. Write a program to declare a string variable `greeting` and assign it the value "Welcome". Then print the value of `greeting`.
2. What does the following code print?  
   ```cpp
   string name = "Alice";
   cout << name;
   ```
3. Modify the above program to ask the user for their name and then greet them by name.
4. Write a program that reads two strings from the user, concatenates them, and then prints the result.
---

### 5.2 String Concatenation

1. Write a program that concatenates the strings "Good" and "Morning" and prints the result.
2. What will the following code output?
   ```cpp
   string firstName = "John";
   string lastName = "Doe";
   cout << firstName + lastName;
   ```
3. Write a program that concatenates a user’s first name and last name with a space between them.

---

### 5.3 Numbers and Strings

1. Write a program that adds two numbers and prints the result.
2. What will this program print?
   ```cpp
   string x = "5";
   string y = "10";
   cout << x + y;
   ```
3. Write a program that concatenates a number (converted to a string) with another string and prints the result.
4. What happens if you try to add an integer and a string, like this:
   ```cpp
   string x = "Hello";
   int y = 5;
   string result = x + y;
   ```
5. Write a program that converts an integer into a string and then concatenates it with another string.
6. Why is adding a number to a string causing an error in the example above?

---

### 5.4 String Length

1. Write a program that prints the length of the string "C++ Programming".
2. What does the following code print?
   ```cpp
   string txt = "OpenAI";
   cout << txt.length();
   ```
3. Write a program that reads a string from the user and prints its length.
4. Explain the difference between `length()` and `size()` for strings.

---

### 5.5 Access Strings

1. Write a program that accesses and prints the first character of the string "Computer".
2. What will the following code output?
   ```cpp
   string greeting = "Hello";
   cout << greeting[2];
   ```
3. Write a program that prints the last character of the string "Programming".
4. Modify the above program to print the third character in the string entered by the user.
5. Write a program that changes the first letter of a string to uppercase and prints the result.
6. Explain what happens when you access a character that is out of range using `myString[index]`.

---

### 5.6 Special Characters

1. Write a program that prints a string containing a double quote ("), like `He said, "Hello!"`.
2. What will this code print?
   ```cpp
   string txt = "It's a beautiful day!";
   cout << txt;
   ```
3. Write a program that demonstrates how to use escape sequences like `\\`, `\'`, and `\"`.
4. What will the following code print?
   ```cpp
   string txt = "He said, \"Hello World!\"";
   cout << txt;
   ```
5. Write a program that prints a string with both single and double quotes, and also contains a newline.
6. Explain why escape characters like `\n` and `\t` are useful when working with strings.

---

### 5.7 User Input Strings

1. Write a program that asks the user for their name and then prints it.
2. What will happen when the following code is run?
   ```cpp
   string name;
   cout << "Enter your name: ";
   cin >> name;
   cout << "Your name is: " << name;
   ```
3. Modify the above program to accept the user’s full name (first and last) and print it.
4. What is the issue with using `cin` to input a full name with spaces?
5. Write a program that accepts a full name from the user (with spaces) using `getline()` and then prints it.
6. Why does `cin` stop reading at the first space, and how can you handle this limitation when reading full names?

---

### 5.8 String Namespace

1. Write a program that uses `std::string` and `std::cout` without using `using namespace std;`.
2. What will the following code output, and why?
   ```cpp
   string greeting = "Hello";
   cout << greeting;
   ```
3. Explain the advantages and disadvantages of using `using namespace std;`.

---

<!--
### 5.9 C-Style Strings

1. Write a program that uses a C-style string (`char[]`) and prints it.
2. What is the difference between a C-style string and a C++ `string`?
3. Write a program that creates a C-style string and prints its length.
4. What is the potential problem with C-style strings compared to C++ strings?
5. Write a program that converts a C-style string to a C++ `string` and prints the result.
6. Why might you prefer to use C++ `string` objects instead of C-style strings in modern C++?
-->

--- 

