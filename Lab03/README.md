# Lab 03 - Python Data Structures & Advanced Functions

This repository contains the solution for **Lab 03**, focusing on efficient data structures, advanced Python built-ins, generator functions, and custom object-oriented implementation (Multiset/Bag) adhering to strict time complexity constraints.

---

## 🛠️ Implemented Features & Functions

1. **`unique_in_order(iterable)`**: 
   - Removes consecutive duplicate elements while preserving the original relative order.
2. **`word_frequencies(text)`**: 
   - Computes case-insensitive word frequencies efficiently using dictionary operations.
3. **`top_k(frequencies, k)`**: 
   - Returns the top $k$ most frequent items, sorted primarily by frequency in descending order and secondarily by alphabetical order in ascending order.
4. **`transpose(matrix)`**: 
   - Transposes a 2D matrix (rows to columns) implemented cleanly using **Nested List Comprehension**.
5. **`invert(mapping)`**: 
   - Inverts a dictionary, grouping original keys under their respective values as sorted lists.
6. **`common_elements(first, second)`**: 
   - Finds the intersection of two iterables using set operations, returning a sorted list of unique common elements.
7. **`group_by_length(words)`**: 
   - Groups words into a dictionary where keys represent word lengths and values are lists of words in their original order.
8. **`Bag` Class (Multiset)**: 
   - A custom multiset data structure storing counts in an internal dictionary. 
   - Designed with performance in mind: **every method (excluding iteration, equality checks, and representation) operates in $O(1)$ time complexity**.
   - Supports custom methods (`add`, `remove`, `count`, `distinct`) and Python magic methods (`__len__`, `__contains__`, `__iter__`, `__eq__`, `__repr__`).
9. **`countdown(n)`**: 
   - A memory-efficient generator yielding numbers from $n$ down to $1$.
10. **`chunks(values, size)`**: 
    - A generator yielding consecutive slices of a collection of a specified size.

---

## 🧪 Running Tests

To run the test suite locally using `pytest`, ensure you are in the directory containing your test files and execute:

```bash
pytest