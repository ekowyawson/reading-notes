# Class 07: Ten Thousand 2

Based on the readings for this class, the important concept here is to understand how to incorporate all of the programming concepts we learned in prior classes into a full Python program: **Ten Thousand** dice game. These concepts include:

- Python scopes
- Big O Notation
- Importing and using Python modules (Random Module)

## [1] Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both

In Python, a variable's **scope** refers to the region of a program where the variable is accessible or "visible." It determines where you can use a variable and whether it's modifiable.
Python follows the **LEGB** rule for variable scope resolution:

- **L**ocal
- **E**nclosing
- **G**lobal
- **B**uilt-in

### Local Scope

Variables defined within a function have local scope. They are accessible only within that function's body and they cease to exist after the function execution ends.

Example:

```python
def my_function():
    x = 10  # Local variable
    print(x)  # Output: 10 (accessible within the function)

my_function()
print(x)  # Error: x is not defined outside the function
```

***NOTE:***

- *Local variables take precedence over global variables with the same name within a function.*

### Global Scope

Variables defined outside any function have global scope. They are accessible from anywhere in the program and they exist throughout the program's execution.

Example:

```python
y = 20  # Global variable

def another_function():
    print(y)  # Output: 20 (accessible from within the function)

another_function()
print(y)  # Output: 20 (accessible outside functions too)
```

***NOTES:***

- *To modify a global variable within a function, use the global keyword.*
- *Avoid excessive use of global variables as they can lead to naming conflicts and make code harder to reason about.*

## [2] How do the global and nonlocal keywords work in Python, and in what situations might you use them?

### Global Keyword

The `global` keyword in Python is used to modify a global variable from within a function. It works by telling Python to treat the variable as global within the function, thereby, allowing you to change the value of the global variable from within the function. If the variable doesn't exist in the global scope, it creates a new global variable.

**Example**:

```python
x = 10  # Global variable

def modify_global():
    global x  # Declare x as global
    x += 5

modify_global()
print(x)  # Output: 15 (global variable has been modified)
```

#### When to use global

You would use `global` when a function genuinely needs to modify a global value that's shared across the program; however, it should be used sparingly as excessive use can make the code less readable and maintainable.

### Nonlocal Keyword

The `nonlocal` keyword in Python is used to modify a variable in an enclosing scope (***not global***) from within a ***nested function***. It works by telling Python to bind the variable to the one in the nearest enclosing scope that is **not** the global scope. This allows you to modify the value of a variable in an enclosing function from within a nested function.

**Example**:

```python
def outer():
    x = 20

    def inner():
        nonlocal x  # Declare x as nonlocal
        x *= 2

    inner()
    print(x)  # Output: 40 (variable in outer scope has been modified)

outer()
```

#### When to use nonlocal

You would use `nonlocal` when you need to modify variables in enclosing scopes within nested functions, often for techniques like `closures`. Use it with caution as it can create hidden dependencies and make the code harder to understand.
Best Practices:

## [3] In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis

### Purpose

Big O notation offers a language-independent way to describe an algorithm's efficiency in terms of how its execution time or memory usage scales with input size. It's not about exact time measurements but about understanding how the algorithm's performance changes as input grows.

By expressing algorithm complexity using Big O notation, you can compare algorithms and make informed choices for different tasks. This aids in predicting how an algorithm will perform with larger inputs, ensuring it can handle real-world data volumes efficiently.

Specifically for us, knowing Big O complexities of Python's built-in data structures and operations allows us to choose appropriate ones for different tasks, leading to more efficient code.

### Importance in Python

Python's dynamic nature makes performance optimization essential. Big O notation helps identify potential performance issues early in development. Its widespread use in data science and machine learning involves handling large datasets, making algorithm efficiency crucial. Big O notation guides algorithm selection for best performance.

## [4] Based on the Rolling Dice Example, explain how you would simulate a dice roll using Python. Describe how you would use code to calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials

### Simulate Rolling of 1000 Dice

```python
import random
count = 0

def roll():
    return random.randint(1,6)

for i in range(1, 1001):
    if roll() == 6:
        count += 1
print(count)
```

Here's a breakdown of how the code simulates a dice roll and calculates probability:

1. *Importing the Random Module*:
   - **`import random`**: This line imports the random module, which provides functions for generating random numbers.
2. *Defining a Roll Function*:
   - **`def roll(): return random.randint(1, 6)`**: This function simulates a single dice roll. It uses `random.randint(1, 6)` to generate a random integer between **1** and **6** (*inclusive*), representing the possible outcomes of a standard 6-sided dice.
3. *Simulating Multiple Rolls*:
   - **`for i in range(1, 1001): ...`**: This loop simulates 1000 dice rolls. It iterates **1000** times, and within each iteration, it calls the `roll()` function to simulate a single roll.
4. *Counting Specific Outcomes*:
   - **`if roll() == 6: count += 1`**: Inside the loop, this conditional statement checks if the result of the roll is **6**. If it is, the count variable is incremented by **1**, keeping track of the number of times a **6** is rolled.
5. *Printing the Count*:
   - **`print(count)`**: After the loop completes, the value of `count` is printed, indicating the total number of times a **6** was rolled in the **1000** trials.

### Calculating Probability

To calculate the probability of rolling a **6**, divide the number of successful outcomes (6s) by the total number of trials: `probability = count / 1000`. This gives you an estimate of the probability based on the simulated trials.

***NOTES***:

- The `random.randint()` function is essential for generating random numbers to simulate dice rolls.
- The loop allows you to repeat the roll multiple times to gather data for probability calculations.
- The conditional statement tracks specific outcomes of interest.
- The probability is calculated by dividing the favorable outcomes by the total trials.

## Sources

- [Python Scope](https://realpython.com/python-scope-legb-rule/)
- [Big O notation is simpler than you might think](https://www.youtube.com/watch?v=dNorFNlDbX0)
- [Rolling Dice Examples](https://web.archive.org/web/20220608035657/https://artofproblemsolving.com/wiki/index.php/Basic_Programming_With_Python#Random)
- ChatGPT

## Things I want to know more about

Nothing at this moment.
