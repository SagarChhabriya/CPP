# C++ User Input

In C++, `cin` is used to receive input from the user. It is a predefined object in the C++ Standard Library that reads data from the keyboard. To extract (receive) input from the user, we use the **extraction operator (>>) with `cin`**.

### Using `cin` for User Input

The general syntax for user input is:

```cpp
cin >> variable;
```

Where `variable` is the name of the variable where the input will be stored.

### Example: Simple User Input

In this simple example, we ask the user to input a number, which is stored in the variable `x`, and then print it:

```cpp
int x;
cout << "Type a number: ";  // Prompt the user to enter a number
cin >> x;                   // Get user input from the keyboard
cout << "Your number is: " << x; // Output the input number
```

**Explanation:**
- `cout`: Used to display the message prompting the user to enter a value.
- `cin`: Used to take the user input and store it in the variable `x`.
- `<<` and `>>`: These are the insertion (for output) and extraction (for input) operators, respectively.

### Good to Know
- **`cout`** is pronounced "see-out", used for output, and uses the **insertion operator (<<)**.
- **`cin`** is pronounced "see-in", used for input, and uses the **extraction operator (>>)**.

### Example: Simple Calculator

Now, let's create a simple calculator where the user can input two numbers, and the program will display their sum:

```cpp
int x, y; // Declare two integer variables
int sum;  // Declare a variable to store the sum
cout << "Type a number: "; // Prompt user for first number
cin >> x;  // Get user input for the first number
cout << "Type another number: "; // Prompt user for second number
cin >> y;  // Get user input for the second number
sum = x + y; // Calculate the sum
cout << "Sum is: " << sum; // Output the sum
```

**Explanation:**
- `x` and `y`: Variables to store the numbers entered by the user.
- `sum`: A variable to store the result of adding `x` and `y`.
- The user is prompted to enter two numbers, and the sum is calculated and printed.

### Summary
- **`cin`** allows you to read user input in C++.
- It uses the **extraction operator (>>) to receive data from the user**.
- **`cout`** is used for displaying output.
- You can create interactive programs, like a calculator, by using `cin` to gather user input and `cout` to display the result.

This is the basic way to handle user input and output in C++.
