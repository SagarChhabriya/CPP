# C++ Beginner Game Questions (Step-by-Step with Expected Output)

---

### 1. **Number Guessing Game**

**Question:**

- Declare an integer `secretNumber = 7`.
- Ask the user to guess a number between 1 and 10.
- Keep asking until the user guesses correctly.
- Give hints: "Too high" or "Too low".

**Expected Output (example run):**
```
Guess a number between 1 and 10: 4  
Too low!  
Guess a number between 1 and 10: 9  
Too high!  
Guess a number between 1 and 10: 7  
Correct! You win!
```

---

### 2. **Odd or Even Checker**

**Question:**

- Ask the user to input a number.
- Use `if-else` to check whether the number is even or odd.
- Ask if they want to try again (y/n).
- Repeat based on user response.

**Expected Output:**
```
Enter a number: 8  
That’s even!  
Try again? (y/n): y  
Enter a number: 5  
That’s odd!  
Try again? (y/n): n  
Thanks for playing!
```

---

### 3. **Mini Quiz Game (3 Questions)**

**Question:**

- Ask 3 multiple-choice questions (a/b/c).
- Use `if` statements to check answers.
- Track the score in an `int score` variable.
- Show final score after 3 questions.

**Expected Output:**
```
Q1. What is 5 + 3?  
a) 6  b) 8  c) 9  
Your answer: b  

Q2. Which planet is known as the Red Planet?  
a) Mars  b) Venus  c) Saturn  
Your answer: a  

Q3. What is the capital of France?  
a) Paris  b) Rome  c) Madrid  
Your answer: a  

You got 3 out of 3 correct!
```

---

### 4. **Simple Calculator Menu**

**Question:**

- Show a menu:
  1. Add  
  2. Subtract  
  3. Multiply  
  4. Divide  
  5. Exit  
- Use `switch` to perform the selected operation.
- Ask for two numbers.
- Loop until user selects Exit.

**Expected Output:**
```
--- Calculator ---
1. Add
2. Subtract
3. Multiply
4. Divide
5. Exit
Enter your choice: 1  
Enter two numbers: 10 5  
Result: 15  

Enter your choice: 4  
Enter two numbers: 8 2  
Result: 4  

Enter your choice: 5  
Exiting calculator...
```

---

### 5. **Text Adventure (Choose Your Path)**

**Question:**

- Print a simple scenario.
- Ask the player to choose `left` or `right`.
- Use `if-else` with strings to determine the outcome.

**Expected Output:**
```
You are standing at a fork in the road.  
Do you go left or right? left  
You find a village and are safe!

(OR another run:)
Do you go left or right? right  
You fall into a trap. Game over!
```

---

### 6. **Countdown Timer (While Loop)**

**Question:**

- Declare `int timer = 5;`
- Use a `while` loop to count down from 5 to 1.
- Print “Time’s up!” at the end.

**Expected Output:**
```
Countdown: 5  
Countdown: 4  
Countdown: 3  
Countdown: 2  
Countdown: 1  
Time’s up!
```

---

### 7. **Password Retry System**

**Question:**

- Set a correct password, e.g., `"admin123"`.
- Allow 3 attempts max.
- On correct password: "Access granted".
- On 3 wrong attempts: "Access denied".

**Expected Output:**
```
Enter password: admin  
Incorrect. Try again.  
Enter password: 1234  
Incorrect. Try again.  
Enter password: admin123  
Access granted!

(OR for failure:)
Enter password: user  
Incorrect. Try again.  
Enter password: guess  
Incorrect. Try again.  
Enter password: hello  
Access denied!
```

---

### 8. **Level Progression Bar**

**Question:**

- Ask user for current level (1 to 10).
- Print progress bar: filled with `#`, empty with `-`.
- Example: level 4 → `####------`

**Expected Output:**
```
Enter your level (1 to 10): 4  
Level Progress: [####------]
```

