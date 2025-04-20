# C++ Loops

## What are Loops in C++?

Loops in C++ allow you to execute a block of code repeatedly as long as a specific condition is met.

### Types of Loops in C++:
1. For Loop
2. While Loop
3. Do-While Loop
4. Nested Loops
5. Range-Based For Loop (C++11 and later)

---

## 1. For Loop

### Syntax:

```cpp
for (initialization; condition; increment/decrement) {
    // code to be executed
}
```

### Example:

```cpp
#include <iostream>
using namespace std;

int main() {
    for (int i = 1; i <= 5; i++) {
        cout << "Iteration " << i << endl;
    }
    return 0;
}
```

Output:
```
Iteration 1
Iteration 2
Iteration 3
Iteration 4
Iteration 5
```

### Practice Questions:
1. Print numbers from 1 to 100.
2. Print numbers from 100 to 1.
3. Print the multiplication table of a given number.
  - Example:
  
  ```mathematica
  Multiplication Table for 2
  2 x 1 = 2
  2 x 2 = 4
  2 x 3 = 6
  2 x 4 = 8
  2 x 5 = 10
  2 x 6 = 12
  2 x 7 = 14
  2 x 8 = 16
  2 x 9 = 18
  2 x 10 = 20
  ```

3. Find the factorial of a number using a for loop.
4. Print the sum of the first `n` natural numbers.

---

## 2. While Loop

### Syntax:

```cpp
while (condition) {
    // code to execute
}
```

### Example:

```cpp
#include <iostream>
using namespace std;

int main() {
    int i = 1;
    while (i <= 5) {
        cout << i << " ";
        i++;
    }
    return 0;
}
```

Output:
```
1 2 3 4 5
```

### Practice Questions:
1. Implement a simple calculator that runs until the user exits.

---

## 3. Do-While Loop

### Syntax:

```cpp
do {
    // code to execute
} while (condition);
```

Note: A do-while loop executes at least once, even if the condition is false at the start.

### Example:

```cpp
#include <iostream>
using namespace std;

int main() {
    int i = 1;
    do {
        cout << i << " ";
        i++;
    } while (i <= 5);
    return 0;
}
```

Output:
```
1 2 3 4 5
```

### Practice Questions:
Sure! Below are the output examples for each of the practice questions you mentioned, showing **both success and failure scenarios**.

---

### **1. ATM Menu - Menu-Driven Program**
#### **Example 1:**
```
===== ATM MENU =====
1. Check Balance
2. Deposit Money
3. Withdraw Money
4. Exit
Enter your choice: 2
Enter amount to deposit: 500
Amount deposited successfully!

===== ATM MENU =====
1. Check Balance
2. Deposit Money
3. Withdraw Money
4. Exit
Enter your choice: 1
Your current balance is: $500
```

#### **Example 2:**
```
===== ATM MENU =====
1. Check Balance
2. Deposit Money
3. Withdraw Money
4. Exit
Enter your choice: 5
Invalid choice! Please select a valid option.

Enter your choice: 3
Enter amount to withdraw: 1000
Insufficient balance!
```

---

### **2. Accept integers until a negative number is entered**
#### **Example 1:**
```
Enter a number: 5
Enter a number: 12
Enter a number: 8
Enter a number: -1
Input stopped. Negative number entered.
```

#### ** Example 2 (invalid input or assumption):**
```
Enter a number: hello
Invalid input! Please enter an integer.
Enter a number: -3
Input stopped. Negative number entered.
```

---

### **3. Number Guessing Game**
_(Let's assume the random number is 7)_

####  **Example 1:**
```
Guess the number (between 1 and 10): 5
Too low. Try again.
Guess the number (between 1 and 10): 9
Too high. Try again.
Guess the number (between 1 and 10): 7
Congratulations! You guessed the correct number.
```

#### **Example 2 (too many wrong attempts or input issues):**
```
Guess the number (between 1 and 10): ten
Invalid input! Please enter a number.
Guess the number (between 1 and 10): 3
Too low. Try again.
Guess the number (between 1 and 10): 6
Too low. Try again.
Guess the number (between 1 and 10): 8
Too high. Try again.
(You can optionally limit attempts and then show a game over message.)
```

---

### **4. Display a Menu Repeatedly Until Exit**
#### ** Example 1:**
```
==== MAIN MENU ====
1. Say Hello
2. Say Goodbye
3. Exit
Enter your choice: 1
Hello there!

==== MAIN MENU ====
1. Say Hello
2. Say Goodbye
3. Exit
Enter your choice: 2
Goodbye!

==== MAIN MENU ====
1. Say Hello
2. Say Goodbye
3. Exit
Enter your choice: 3
Exiting program. Goodbye!
```

####  **Failure Example: 2**
```
==== MAIN MENU ====
1. Say Hello
2. Say Goodbye
3. Exit
Enter your choice: 9
Invalid option. Please try again.

==== MAIN MENU ====
1. Say Hello
2. Say Goodbye
3. Exit
Enter your choice: hello
Invalid input! Please enter a number.
```



## 4. Nested Loops

### Syntax:

```cpp
for (int i = 0; i < n; i++) {
    for (int j = 0; j < m; j++) {
        // code
    }
}
```

### Example: Pattern Printing

```cpp
#include <iostream>
using namespace std;

int main() {
    for (int i = 1; i <= 3; i++) {
        for (int j = 1; j <= 3; j++) {
            cout << "* ";
        }
        cout << endl;
    }
    return 0;
}
```

Output:
```
* * * 
* * * 
* * * 
```

### Practice Questions:
1. Print various star/pyramid patterns.
- **Right-Angled Triangle Pattern**

```markdown
Enter number of rows: 5

*
**
***
****
*****

```

- **Pyramid Pattern**
```markdown
Enter number of rows: 4

   *
  ***
 *****
*******

```
- Invalid Input Example


```pgsql
Enter number of rows: -3
Invalid input! Number of rows must be positive.
```

```pgsql
Enter number of rows: -3
Invalid input! Number of rows must be positive.
```

 

---

## 5. Range-Based For Loop (C++11 and Later)

### Syntax:

```cpp
for (datatype variable : container) {
    // code
}
```

### Example:

```cpp
#include <iostream>
#include <vector>
using namespace std;

int main() {
    vector<int> nums = {1, 2, 3, 4, 5};
    for (int num : nums) {
        cout << num << " ";
    }
    return 0;
}
```

Output:
```
1 2 3 4 5
```

### Practice Questions: (Solve these After Learning Vectors)
1. Calculate the average of numbers in a vector. 
2. Count positive and negative numbers using a range-based loop. 
3. Print each character in a string.
4. Convert all lowercase characters in a string to uppercase.

---

## Loop Control Statements

### `break` Statement

Used to exit a loop prematurely when a certain condition is met.

```cpp
for (int i = 1; i <= 10; i++) {
    if (i == 5) break;
    cout << i << " ";
}
```

Output:
```
1 2 3 4
```

### `continue` Statement

Skips the current iteration and moves to the next one.

```cpp
for (int i = 1; i <= 5; i++) {
    if (i == 3) continue;
    cout << i << " ";
}
```

Output:
```
1 2 4 5
```

---

## Bonus Practice Problems

1. Count even and odd numbers from 1 to N.
2. Print all divisors of a number.

3. Check if a number is an Armstrong number.

4. Rotate elements in an string using loops.
   - Input: `sagar`
   - Output: `ragas`

5. Check if a string is palindrome or not
   - Palindrome: The original string and its reverse are the same.
     - Ex: `bob` and the reverse of `bob` are same. `paisa` and the reverse `asiap` are not same (Not Palindrome). 
