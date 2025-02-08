# C++ Strings
Strings are used for storing text/characters.

- For example, "Hello World" is a string.
- A string variable contains a collection of characters surrounded by double quotes:


## 5.1 Strings Introduction

### Example
Create a variable of type string and assign it a value:

```cpp
string greeting = "Hello";
```

- To use strings, you must include an additional header file in the source code, the <string> library:

### Example

```cpp
// Include the string library
#include <string>

// Create a string variable
string greeting = "Hello";
```



## 5.2 String Concatenation
The + operator can be used between strings to add them together to make a new string. This is called concatenation:

### Example

```cpp
string firstName = "John ";
string lastName = "Doe";
string fullName = firstName + lastName;
cout << fullName;
```

In the example above, we added a space after firstName to create a space between John and Doe on output. However, you could also add a space with quotes (" " or ' '):

### Example

```cpp
string firstName = "John";
string lastName = "Doe";
string fullName = firstName + " " + lastName;
cout << fullName;

```
<!-- 
## Append
A string in C++ is actually an object, which contain functions that can perform certain operations on strings. For example, you can also concatenate strings with the append() function:

### Example

string firstName = "John ";
string lastName = "Doe";
string fullName = firstName.append(lastName);
cout << fullName; -->




## 5.3 Numbers and Strings

- Adding Numbers and Strings
- C++ uses the + operator for both addition and concatenation.
- Numbers are added. Strings are concatenated.

- If you add two numbers, the result will be a number:

### Example

```cpp
int x = 10;
int y = 20;
int z = x + y;      // z will be 30 (an integer)
```

If you add two strings, the result will be a string concatenation:

### Example

```cpp
string x = "10";
string y = "20";
string z = x + y;   // z will be 1020 (a string)

```
If you try to add a number to a string, an error occurs:

### Example

```cpp
string x = "10";
int y = 20;
string z = x + y;
 ```


## 5.4 String Length
To get the length of a string, use the length() function:

### Example

```cpp
string txt = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
cout << "The length of the txt string is: " << txt.length();
```

Tip: You might see some C++ programs that use the size() function to get the length of a string. This is just an alias/othername of length(). It is completely up to you if you want to use length() or size():

### Example

```cpp
string txt = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
cout << "The length of the txt string is: " << txt.size();
```

## 5.5 Access Strings
You can access the characters in a string by referring to its index number inside square brackets [].

### Example: This example prints the first character in myString:

```cpp
string myString = "Hello";
cout << myString[0];
// Outputs H
```

Note: String indexes start with 0: [0] is the first character. [1] is the second character, etc.

This example prints the second character in myString:

### Example

```cpp
string myString = "Hello";
cout << myString[1];
// Outputs e
```

To print the last character of a string, you can use the following code:

### Example

```cpp
string myString = "Hello";
cout << myString[myString.length() - 1];
// Outputs o
```

### Change String Characters
To change the value of a specific character in a string, refer to the index number, and use single quotes:

### Example

```cpp
string myString = "Hello";
myString[0] = 'J';
cout << myString;
// Outputs Jello instead of Hello
```

### Example

```cpp
string myString = "Hello";
cout << myString; // Outputs Hello

cout << myString.at(0);  // First character
cout << myString.at(1);  // Second character
cout << myString.at(myString.length() - 1);  // Last character

myString.at(0) = 'J';
cout << myString;  // Outputs Jello
```

## 5.6 Special Characters
Because strings must be written within quotes, C++ will misunderstand this string, and generate an error:

```cpp
string txt = "We are the so-called "Vikings" from the north.";
```

- The solution to avoid this problem, is to use the backslash escape character.
- The backslash (\\) escape character turns special characters into string characters:

|   Escape character	|   Result  |	Description |
|-----------------------|-----------|---------------|
|   \\'	                |   '	    |   Single quote|
|   \\"	                |   "	    |   Double quote|
|   \\\	                |   \	    |   Backslash   |

The sequence \\"  inserts a double quote in a string:


### Example

```cpp
string txt = "We are the so-called \"Vikings\" from the north.";
```

The sequence \\'  inserts a single quote in a string:


### Example

```cpp
string txt = "It\'s alright.";
```
The sequence \\\  inserts a single backslash in a string:


### Example

```cpp
string txt = "The character \\ is called backslash.";
```

Other popular escape characters in C++ are:

|   Escape Character    |	Result	    |
|-----------------------|---------------|
|   \n	                |   New Line	|
|   \t	                |   Tab         |


## 5.7 User Input Strings
It is possible to use the extraction operator >> on cin to store a string entered by a user:

### Example

```cpp
string firstName;
cout << "Type your first name: ";
cin >> firstName; // get user input from the keyboard
cout << "Your name is: " << firstName;

// Type your first name: John
// Your name is: John
```

However, cin considers a space (whitespace, tabs, etc) as a terminating character, which means that it can only store a single word (even if you type many words):

### Example

```cpp
string fullName;
cout << "Type your full name: ";
cin >> fullName;
cout << "Your name is: " << fullName;

// Type your full name: John Doe
// Your name is: John
```

- From the example above, you would expect the program to print "John Doe", but it only prints "John".

- That's why, when working with strings, we often use the getline() function to read a line of text. It takes cin as the first parameter, and the string variable as second:

### Example

```cpp
string fullName;
cout << "Type your full name: ";
getline (cin, fullName);
cout << "Your name is: " << fullName;

// Type your full name: John Doe
// Your name is: John Doe
```


## 5.8 String Namespace
You might see some C++ programs that run without the standard namespace library. The using namespace std line can be omitted and replaced with the std keyword, followed by the :: operator for string (and cout) objects:

### Example

```cpp
#include <iostream>
#include <string>
// using namespace std; - Remove this line

int main() {
  std::string greeting = "Hello";
  std::cout << greeting;
  return 0;
}
```

It is up to you if you want to include the standard namespace library or not.

## 5.9 C-Style Strings
- C-style strings are created with the char type instead of string.

- The name comes from the C language, which, unlike many other programming languages, does not have a string type for easily creating string variables. Instead, you must use the char type and create an array of characters to make a "string" in C.

- As C++ was developed as an extension of C, it continued to support this way of creating strings in C++:

### Example

```cpp
string greeting1 = "Hello";  // Regular String
char greeting2[] = "Hello";  // C-Style String (an array of characters)
```

> Note: It is more convenient to work with the standard string type, rather than C-style strings. However, one reason some users continue to use C-style strings is that they have access to functions from the C standard library.
