# Lab 02 — Control Flow, Functions, Errors, and Modules

This repository contains the solution for **Lab 02** of the Data Structures and Algorithms coursework, focusing on control flow structures, custom functions, error handling, and python modules.

---

## 🛠️ Lab Contents & Functions

The lab is divided into three main sections:

### 1. Decisions (`-- decisions`)
* **`classify_triangle(a, b, c)`**: Validates triangle side lengths (positive numbers and triangle inequality theorem) and returns whether it's `"equilateral"`, `"isosceles"`, or `"scalene"`.
* **`course_result(coursework, final, attendance)`**: Implements course grading rules, checking attendance thresholds (barred), final exam marks, and total scores to determine pass/fail status.

### 2. Loops (`-- loops`)
* **`fizzbuzz(n)`**: Generates the classic FizzBuzz sequence up to $n$ as a list of strings.
* **`is_prime(n)`**: Checks if a given number is prime efficiently using square-root optimization.
* **`primes_below(n)`**: Returns all prime numbers strictly less than $n$ in increasing order.
* **`first_repeated(values)`**: Finds the first element in a list that repeats an earlier element.
* **`count_pairs(n)`**: Computes nested loop iteration counts using an $O(1)$ mathematical formula.
* **`calculator(command)`**: Evaluates a miniature command-line language supporting operations (`add`, `mul`, `neg`, `sum`) using `match` statements.

### 3. Functions (`-- functions`)
* **`parse_int(text, default=None)`**: Safely converts text to an integer using `try/except` blocks, falling back to a default value on failure.
* **`stats(*numbers)`**: Computes the minimum, maximum, and mean of a variable number of arguments without using built-in aggregation functions (`min`, `max`, `sum`).
* **`append_to(item, target=None)`**: Avoids the mutable default argument trap by initializing a new list when none is provided.
* **`make_multiplier(k)`**: A higher-order function that returns a custom multiplier function.
* **`apply_n(f, x, n)`**: Applies a given function $f$ to an input $x$ recursively $n$ times ($f(f(\dots f(x)\dots))$).

---

## 🚀 Running the Tests

To verify the implementation, the provided `pytest` suite can be executed from the terminal:

```bash
pytest tests/test_lab02.py -v