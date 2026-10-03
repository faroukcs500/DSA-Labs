# Lab 01 - Python Foundations & Problem Solving

This repository contains the complete implementation for **Lab 01**, covering essential Python programming concepts including string formatting, list operations, mathematical logic, and recursion/loops. All functions have been implemented from scratch and verified using unit tests.

---

## Repository Structure

- labs/
  - __init__.py
  - lab01.py          (Core function implementations)
- test_lab01.py         (Pytest test suite)
- README.md             (Project documentation)

---

## Detailed Function Breakdown

The `labs/lab01.py` file includes the following function implementations:

1. `seconds_to_hms(seconds)`
   - Converts total seconds into a formatted string `H:MM:SS`.
   - Formats minutes and seconds with leading zeros for single-digit values.

2. `celsius_to_fahrenheit(celsius)`
   - Converts temperature from Celsius to Fahrenheit using the formula `(C * 9/5) + 32`.
   - Returns the value rounded to 1 decimal place.

3. `split_evenly(total, people)`
   - Calculates the integer share per person and the remaining leftover amount.
   - Returns a tuple `(share, left_over)`.

4. `initials(full_name)`
   - Extracts the first letter of each word in a name, converts it to uppercase, and appends a period (e.g., `"H.E."`).
   - Ignores extra spaces between names.

5. `is_palindrome_word(word)`
   - Checks if a word reads the same forwards and backwards (case-insensitive and ignores leading/trailing whitespaces).

6. `mask_email(email)`
   - Masks the username part of an email address with asterisks `*`, keeping only the first and last character of the username (e.g., `h*****m@example.com`).
   - Leaves usernames with length <= 2 unmasked.

7. `middle(values)`
   - Returns the middle element(s) of a list:
     - Returns an empty list `[]` if the input list is empty.
     - Returns a list with the single middle element if the length is odd.
     - Returns a list with the two middle elements if the length is even.

8. `rotate_left(values, k)`
   - Rotates a list to the left by `k` positions.
   - Handles cases where `k` is larger than the list length using modulo arithmetic (`k % len`).

9. `fib_list(n)`
   - Generates a list containing the first `n` numbers of the Fibonacci sequence starting from `0`.

10. `collatz_steps(n)`
    - Calculates the number of steps required to reach `1` according to the Collatz conjecture (halve if even, `3n + 1` if odd).
    - Raises a `ValueError` for inputs less than `1`.

---

## Testing

All implementations are tested against multiple test cases using `pytest`.

### Prerequisites
Make sure `pytest` is installed:
pip install pytest

### Running Tests
To run all test cases, execute:
pytest test_lab01.py

---

## Author
FAROUK MUHAMMED