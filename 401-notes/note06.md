# Class 06: Ten Thousand Game 1

Based on the readings for this class, the important concept here is to understand how to incorporate all programming concepts learned from prior classes into a full python program. These concepts include:

- Importing and using Python modules (Random Module)
- Incorporating tests and test coverage
- Big O Notation
- Dependency Injection

A new concept introduced is Risk Assessment.

## [1] How can the `random` module be utilized in Python to generate random numbers or make selections from a list, and what are some common functions available within the module?

Python's `random` module generates pseudorandom numbers, meaning they are not truly random but are determined by a mathematical algorithm. Use of the module is generally suitable for most practical applications.

### Module Usage

To use Python's `random` module, you would:

- Import it into your project

```python
import random
```

- Implement logic to generate random numbers:
  - **`random.random()`**: Generates a random floating-point number between 0 and 1 (exclusive of 1).

    ```python
    random_float = random.random()  # Example: 0.7354923754
    ```

  - **`random.randint(a, b)`**: Generates a random integer between a (inclusive) and b (inclusive).
  
    ```python
    random_integer = random.randint(1, 10)  # Example: 7
    ```

- Implement logic to make selections from lists:
  - `random.choice(sequence)`: Chooses a random element from a sequence (like a list or tuple).

    ```python
    fruits = ["apple", "banana", "orange"]
    random_fruit = random.choice(fruits)  # Example: "banana"
    ```

  - **`random.shuffle(sequence)`**: Shuffles the elements of a list in-place, randomly reordering them.

    ```python
    random.shuffle(fruits)  # Example: fruits becomes ["orange", "apple", "banana"]
    ```

  - **`random.sample(population, k)`**: Returns a new list containing k unique elements chosen randomly from the population sequence.

    ```python
    random_sample = random.sample(fruits, 2)  # Example: ["apple", "orange"]
    ```

- Other common functions include:
  - **`random.seed(x)`**: Sets the seed for the random number generator, ensuring the same sequence of numbers is generated each time the program runs with the same seed value.
  - **`random.uniform(a, b)`**: Generates a random floating-point number between `a` (*inclusive*) and `b` (*exclusive*).
  - **`random.randrange(start, stop, step)`**: Returns a randomly selected element from `range(start, stop, step)`.

## [2] In the context of software development, what is *risk analysis*, and what are the key steps involved in conducting a risk analysis for a software project?

According to the article [What is Risk Analysis](https://www.edureka.co/blog/risk-analysis-in-software-testing/), risk analysis is the process of identifying and prioritizing risks in software applications. It involves assessing the likelihood and impact of potential problems so that they can be mitigated. Risks can arise from a variety of factors, such as new technology, tight deadlines, or incomplete requirements. By identifying and addressing risks early in the development process, software testers can help to ensure that the software is delivered on time and within budget.

There are three key steps involved in conducting a risk analysis for a software project:

1. Searching for the risk.
2. Analyzing the impact of each individual risk.
3. Taking measures for the risk identified.

## [3] What is test coverage and why is it an important (or potentially misleading) metric in software testing?

Test coverage is a metric that measures the percentage of code that is covered by tests. It is often used as a way to gauge the quality of a test suite, but it can be a misleading metric.

There are a number of reasons why test coverage can be misleading. ***First***, it is possible to achieve high coverage numbers with low-quality tests that do not actually test the important parts of the code. ***Second***, focusing on coverage can lead developers to write tests that are simply designed to increase the coverage numbers, rather than tests that are designed to find bugs. ***Third***, high coverage numbers can give a false sense of security, leading developers to believe that their code is well-tested when it may not be.

Despite these limitations, test coverage can still be a useful tool if it is used correctly. It can help to identify areas of code that are not being tested, and it can be used to track progress over time. However, it is important to remember that test coverage is just one metric, and it should not be used as the sole measure of the quality of a test suite.

## [4] What is Big O notation, and how is it used to describe the performance of an algorithm? Give an example of an everyday task (not software related) that demonstrates O(n) time complexity

**Big O notation** is a mathematical notation used to describe the approximate growth of the **time** or **space** **complexity** of an algorithm as its input size (**n**) increases. It focuses on the ***worst-case scenario***, helping us understand how an algorithm might scale as it handles larger inputs. Big 'O' doesn't provide exact timings, but rather a way to compare the efficiency of different algorithms.

### Common Big O Notations

- **O(1)**: *Constant time* - input size doesn't affect time complexity (e.g., checking the first item in a list).
- **O(n)**: *Linear time* - time complexity grows directly proportional to input size (e.g., searching for a name in a phone book).
- **O(n^2)**: *Quadratic time* - time complexity grows as the square of input size (e.g., comparing each item in a list with every other item).
- **O(log n)**: *Logarithmic time* - time complexity grows logarithmically with input size (e.g., finding a word in a dictionary using binary search).

### Everyday Example of O(n) Time Complexity

**Task**: Waiting in a single-line queue to buy tickets.

**Input size (*n*)**: Number of people in the queue ahead of you.

**Time complexity**: ***O(n)*** because the time you spend waiting increases linearly with the number of people ahead of you.

**Explanation**:

If there's one person ahead of you, you'll wait for their transaction. If there are five people, you'll wait for five transactions. The time you spend grows directly proportional to the number of people in the queue.

## Sources

- [How to use Random Module](https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)
- [What is Risk Analysis](https://www.edureka.co/blog/risk-analysis-in-software-testing/)
- [Test Coverage](https://martinfowler.com/bliki/TestCoverage.html)
- [Big O Notation](https://www.youtube.com/watch?v=v4cd1O4zkGw)
- [Python Random](https://docs.python.org/3/library/random.html)
- [What is Dependency Injection](https://www.freecodecamp.org/news/a-quick-intro-to-dependency-injection-what-it-is-and-when-to-use-it-7578c84fa88f/)
- ChatGPT

## Things I want to know more about

Nothing at this moment.
