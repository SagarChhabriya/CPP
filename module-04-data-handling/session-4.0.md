
# C++ Data Types

In C++, every variable must be declared with a specified data type. The data type determines the size and type of information the variable will store.

## Example

```cpp
int myNum = 5;               // Integer (whole number)
float myFloatNum = 5.99;     // Floating point number
double myDoubleNum = 9.98;   // Floating point number
char myLetter = 'D';         // Character
bool myBoolean = true;       // Boolean
string myText = "Hello";     // String
```

## Basic Data Types

The data type specifies the size and type of information a variable will store:

| Data Type | Size     | Description                                          |
|-----------|----------|------------------------------------------------------|
| boolean   | 1 byte   | Stores true or false values                         |
| char      | 1 byte   | Stores a single character/letter/number, or ASCII values |
| int       | 2 or 4 bytes | Stores whole numbers (without decimals)             |
| float     | 4 bytes  | Stores fractional numbers, containing 6-7 decimal digits |
| double    | 8 bytes  | Stores fractional numbers, containing 15 decimal digits |

## C++ Numeric Data Types

### Numeric Types

- Use **int** when you need to store whole numbers without decimals, like `35` or `1000`.
- Use **float** or **double** when you need a floating point number with decimals, like `9.99` or `3.14515`.

### Examples

```cpp
int myNum = 1000;
cout << myNum;

float myNum = 5.75;
cout << myNum;

double myNum = 19.99;
cout << myNum;
```

### Float vs. Double

- **Precision** of a floating-point value indicates how many digits can appear after the decimal point.
- **float** has a precision of about 6-7 decimal digits.
- **double** has a precision of about 15 decimal digits.
- It is generally safer to use **double** for most calculations due to its higher precision.

### Scientific Numbers

A floating-point number can also be represented as a scientific number using an "e" (exponent) to indicate the power of 10:

```cpp
float f1 = 35e3;   // 35 * 10^3
double d1 = 12E4;  // 12 * 10^4

cout << f1;
cout << d1;
```

## C++ Boolean Data Types

### Boolean Types

The **bool** data type can only store two values: `true` or `false`. 

- When `true` is returned, it equals `1`.
- When `false` is returned, it equals `0`.

### Example

```cpp
bool isCodingFun = true;
bool isFishTasty = false;
cout << isCodingFun;  // Outputs 1 (true)
cout << isFishTasty;  // Outputs 0 (false)
```

Boolean values are primarily used for conditional testing, which you will explore later.

### Exercise

Which data type would you use to store true or false values?

- int
- float
- bool
- boolean
- char

## C++ Character Data Types

### Character Types

The **char** data type is used to store a single character. The character must be enclosed in single quotes (`'A'`, `'c'`), and each character is stored as an ASCII value.

### Example

```cpp
char myGrade = 'B';
cout << myGrade;
```

You can also use **ASCII values** to display characters:

```cpp
char a = 65, b = 66, c = 67;
cout << a;  // Outputs 'A'
cout << b;  // Outputs 'B'
cout << c;  // Outputs 'C'
```

## C++ String Data Types

### String Types

In C++, the **string** type is used to store a sequence of characters. Unlike other primitive data types, string is not built-in, but behaves like one in its basic usage. String values must be surrounded by double quotes.

### Example

```cpp
string greeting = "Hello";
cout << greeting;
```

To use strings, include the `<string>` library in your code:

```cpp
#include <string>

string greeting = "Hello";
cout << greeting;
```

You will explore more about strings in C++ in the *C++ Strings* chapter.

## C++ Data Types Real-Life Example

Here’s a practical example of using different data types to calculate and output the total cost of a number of items:

```cpp
// Create variables of different data types
int items = 50;
double cost_per_item = 9.99;
double total_cost = items * cost_per_item;
char currency = '$';

// Print variables
cout << "Number of items: " << items << "\n";
cout << "Cost per item: " << cost_per_item << currency << "\n";
cout << "Total cost = " << total_cost << currency << "\n";
```
